---
title: Problémy s overením
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976864"
---
# <a name="authentication-issues"></a>Problémy s overením

**Hľadáte informácie o kódoch chýb AADSTS vrátených zo služby tokenov zabezpečenia služby Azure Active Directory (Azure AD)?** Popisy chýb AADSTS, opravy a niektoré odporúčané alternatívne riešenia nájdete v téme [Overenie služby Azure AD a kódy chyby overenia](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).

Chyby oprávnenia môžu byť spôsobené niekoľkými rôznymi problémami, z ktorých väčšina vygeneruje chybu 401 alebo 403. K chybám oprávnenia môžu napríklad viesť všetky nasledujúce problémy:

- Nesprávne [toky akvizície prístupového tokenu](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Zle nakonfigurované [rozsahy povolení](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Chýbajúci [súhlas](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Ak chcete vyriešiť bežné chyby oprávnenia, vyskúšajte kroky uvedené nižšie, ktoré sa najviac zhodujú so zobrazenou chybou. Chyba, ktorá sa zobrazuje, možno vyžaduje viac než jeden krok.

**401 – Neoprávnený prístup: Je token platný?**

Uistite sa, že aplikácia v rámci žiadosti uvádza platný prístupový token pre Microsoft Graph. Táto chyba často znamená, že prístupový token môže chýbať v hlavičke požiadavky na overenie HTTP alebo že token je neplatný alebo uplynula jeho platnosť. Na získanie prístupového tokenu dôrazne odporúčame použiť knižnicu overovania spoločnosti Microsoft (MSAL). Okrem toho sa táto chyba môže vyskytnúť, ak sa na prístup k rozhraniu API, ktoré podporuje len pracovné alebo školské kontá (kontá organizácie), pokúsite použiť delegovaný prístupový token udelený osobnému kontu Microsoft.

**Chyba 403 – Zakázané: Vybrali ste správnu množinu povolení?**

Skontrolujte, či ste požiadali o správnu množinu povolení na základe rozhraní API pre Microsoft Graph, ktoré vaša aplikácia volá. Odporúčané povolenia s najmenšími oprávneniami sú k dispozícii vo všetkých témach referenčných metód rozhrania API pre Microsoft Graph. Okrem toho musí tieto povolenia udeliť aplikácii používateľ alebo správca. Udeľovanie povolení sa zvyčajne vykonáva prostredníctvom stránky súhlasu alebo s použitím registračného systému aplikácie Azure Portal. V časti **Nastavenia** v aplikácii kliknite na položku **Požadované povolenia** a potom kliknite na položku **Udeliť povolenia**. Ďalšie informácie nájdete v téme:

- [Povolenia pre Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Informácie o povoleniach a súhlase v službe Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Chyba 403 – Zakázané: Získala vaša aplikácia token, ktorý zodpovedá vybratým povoleniam?**

Skontrolujte, či typy požadovaných alebo udelených povolení zodpovedajú typu prístupového tokenu, ktorý vaša aplikácia získa. Možno požadujete a udeľujete povolenia aplikácie, ale namiesto tokenov toku prihlasovacích údajov klienta používate tokeny toku delegovaných interaktívnych kódov, prípadne požadujete a udeľujete delegované povolenia, ale namiesto tokenov toku delegovaných kódov používate tokeny toku prihlasovacích údajov klienta.

Ďalšie informácie týkajúce sa získania tokenov nájdete v témach:

- [Získanie prístupu v mene používateľov a delegovaných povolení](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – tok kódu oprávenia OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Získanie prístupu bez povolenia používateľa (služby daemon) a aplikácie](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – tok prihlasovacích údajov klienta OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Chyba 403 – Zakázané: Vytvorenie nového hesla**

V súčasnosti nie sú k dispozícii žiadne povolenia služieb deamon pre aplikácie, ktoré by umožňovali vytvoriť nové heslá používateľov. Tieto rozhrania API sú podporované len pomocou tokov interaktívnych delegovaných kódov s prihláseným správcom. Ďalšie informácie nájdete v téme [Povolenia pre Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 Zakázané: Má používateľ prístup a má licenciu?**

V prípade tokov delegovaného kódu Microsoft Graph vyhodnotí, či bola žiadosť povolená na základe povolení udelených aplikácii a povolení, ktoré má prihlásený používateľ. Táto chyba vo všeobecnosti znamená, že používateľ nemá dostatočné oprávnenie na vykonanie požiadavky **alebo** že používateľ nemá licenciu na údaje, ku ktorých chce získať prístup. Úspešnú žiadosť môžu úspešne vykonať iba používatelia s požadovanými povoleniami alebo licenciami.

**403 Zakázané: Vybrali ste správne rozhranie API zdroja?**

Služby API, ako napríklad Microsoft Graph, skontrolujú, či nárok *aud* (cieľová skupina) v prijatom prístupového tokene zodpovedá očakávanej hodnote, a ak nie, vyskytne sa chyba 403 Zakázané. Častou chybou, výsledkom ktorej je táto chyba, je pokus o použitie tokenu získaného pre rozhrania API Azure AD Graph, rozhrania API Outlooku alebo rozhrania API SharePointu/OneDrivu na volanie Microsoft Graph (alebo naopak). Uistite sa, že zdroj (alebo rozsah) vašej aplikácie získava token, ktorý sa zhoduje s rozhraním API, ktoré aplikácia volá.

**400 Nesprávna požiadavka alebo 403 Zakázané: Dodržiava používateľ politiky podmieneného prístupu svojej organizácie?**

Na základe politík podmieneného prístupu (CA) organizácie môže byť používateľ, ktorý má prístup k zdrojom Microsoft Graph prostredníctvom aplikácie, otestovaný s cieľom získať ďalšie informácie, ktoré momentálne nie sú dostupné v prístupovom tokene, ktorý vaša aplikácia pôvodne získala. V tomto prípade sa v aplikácii zobrazí chyba **400 s chybou *interaction_required*** (počas akvizície prístupového tokenu) alebo chyba **403 s chybou *insufficient_claims*** (pri volaní do Microsoft Graph). V oboch prípadoch odpoveď na chybu obsahuje ďalšie informácie, ktoré je možné zobraziť v oprávnenom koncovom bode s cieľom otestovať používateľa s cieľom získať ďalšie informácie (napríklad viacfaktorové overovanie alebo registrácia zariadenia).

Ďalšie informácie týkajúce sa podmieneného prístupu nájdete v témach:

- [Riešenie problémov s podmieneným prístupom pomocou MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Pokyny pre vývojárov pre podmienený prístup k službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Ukončenie podpory pre križnicu Azure Active Directory Authentication Library (ADAL) a rozhranie Azure AD Graph API (AAD Graph)_* _

- Od 30. júna 2020 už nebudeme pridávať žiadne nové funkcie do knižnice Azure Active Directory Authentication Library (ADAL) a rozhrania AD Graph API (AAD Graph). Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.
- Od 30. júna 2022 ukončíme podporu pre ADAL a AAD Graph a nebudeme poskytovať technickú podporu ani aktualizácie zabezpečenia.
    - Aplikácie používajúce ADAL v existujúcich verziách operačného systému budú fungovať aj naďalej, ale nebudú mať k dispozícii žiadnu technickú podporu ani aktualizácie zabezpečenia.
    - Aplikácie používajúce AAD Graph po tomto čase už nemusia prijímať odpovede z koncového bodu AAD Graphu.

_ *Migrácia ADAL**

Odporúčame aktualizovať na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) s najnovšími funkciami a aktualizáciami zabezpečenia. Pri tomto odporúčaní ide o migráciu aplikácií spoločnosti Microsoft do MSAL do termínu ukončenia podpory. Cieľom migrácie aplikácií spoločnosti Microsoft do MSAL je zabezpečiť, aby aplikácie mohli využívať výhody priebežného zabezpečenia a vylepšení funkcií pre MSAL.

- [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Informácie o migrácii aplikácií na platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ak potrebujete pomoc s pochopením toho, ktoré aplikácie používajú ADAL, odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a v prípade potreby kontaktovať všetkých nezávislých dodávateľov softvéru alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.

**Migrácia AAD Graph**

V prípade aplikácií, ktoré používajú AAD Graph, postupujte podľa našich pokynov na [migráciu aplikácií Azure AD Graph do služby Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Náš kontrolný zoznam migrácie obsahuje informácie na začiatok](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Portál registrácie aplikácie Azure zobrazuje aplikácie, ktoré používajú AAD Graph. Odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a v prípade potreby kontaktovať poskytovateľov internetových služieb alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám môže poskytnúť aj informácie o používaní AAD Graphu v nájomníkovi.

 










