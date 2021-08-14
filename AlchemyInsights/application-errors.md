---
title: Chyby aplikácie
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931464"
---
# <a name="application-errors"></a>Chyby aplikácie

Hľadáte informácie o kódoch **chýb AADSTS,** ktoré sa vrátia zo služby tokenu zabezpečenia pre Azure Active Directory (Azure AD)? Prečítajte [si článok Kódy chýb overovania a](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) oprávnenia v Azure AD a vyhľadajte popisy chýb AADSTS, opravy a niektoré navrhované alternatívne riešenia.

Chyby oprávnenia môžu byť spôsobené niekoľkými rôznymi problémami, z ktorých väčšina vygeneruje chybu 401 alebo 403. Chyby v oprávneniach môžu viesť napríklad k týmto chybám:

- Nesprávne [toky akvizície prístupového tokenu](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Zle nakonfigurované [rozsahy povolení](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Chýbajúci [súhlas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Na vyriešenie bežných chýb oprávnenia vyskúšajte nižšie uvedené kroky, ktoré najviac zodpovedajú chybe, ktorá sa vám zobrazuje. Môže sa to vzťahovať na viacero.

**401 – Neoprávnený prístup: Je token platný?**

Presvedčte sa, že vaša aplikácia v rámci žiadosti prezentuje platný prístupový token Graph Spoločnosti Microsoft. Táto chyba často znamená, že prístupový token môže chýbať v hlavičke požiadavky na overenie HTTP alebo že token je neplatný alebo uplynula jeho platnosť. Na získanie prístupového tokenu [dôrazne odporúčame použiť knižnicu Microsoft Authentication Library (MSAL).](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) Táto chyba sa môže vyskytnúť aj vtedy, ak sa pokúsite použiť delegovaný prístupový token udelený pre osobné konto Microsoft na prístup k rozhraniu API, ktoré podporuje iba pracovné alebo školské kontá (kontá organizácie).

**Chyba 403 – Zakázané: Vybrali ste správnu množinu povolení?**

Skontrolujte, či ste požiadali o správnu množinu povolení podľa rozhraní Microsoft Graph API vašich hovorov z aplikácie. Odporúčané najmenej privilegované povolenia sú k dispozícii vo všetkých témach s referenčnou Graph rozhrania API spoločnosti Microsoft. Okrem toho musí tieto povolenia udeliť aplikácii používateľ alebo správca. Udelenie povolení sa zvyčajne vykonáva prostredníctvom stránky so súhlasom alebo udelením povolení pomocou aplikácie Azure Portal registration blade. V časti **Nastavenia** v aplikácii kliknite na položku **Požadované povolenia** a potom kliknite na položku **Udeliť povolenia**.

- [Povolenia pre Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Informácie o povoleniach a súhlase v službe Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Chyba 403 – Zakázané: Získala vaša aplikácia token, ktorý zodpovedá vybratým povoleniam?**

Uistite sa, že typ požadovaných alebo udelených povolení zodpovedá typu prístupového tokenu, ktorý vaša aplikácia získava. Môžete požiadať o povolenia aplikácie a udeliť ich, no namiesto tokenov toku poverení klienta budete namiesto tokenov toku poverení klienta používať delegované tokeny toku poverení, ale namiesto tokenov toku delegovaných kódov budete používať tokeny toku poverení klienta.

- [Získanie prístupu v mene používateľov a delegovaných povolení](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – tok kódu oprávenia OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Získanie prístupu bez povolenia používateľa (služby daemon) a aplikácie](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – tok prihlasovacích údajov klienta OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Chyba 403 – Zakázané: Vytvorenie nového hesla**

V súčasnosti nie sú k dispozícii žiadne povolenia služieb deamon pre aplikácie, ktoré by umožňovali vytvoriť nové heslá používateľov. Tieto rozhrania API sú podporované len pomocou tokov interaktívnych delegovaných kódov s prihláseným správcom.

- [Povolenia pre Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 Zakázané: Má používateľ prístup a má licenciu?**

V prípade tokov delegovaných kódov spoločnosť Microsoft Graph vtedy, ak je žiadosť povolená na základe povolení udelených pre aplikáciu a povolení, ktoré má prihlásený používateľ. Táto chyba vo všeobecnosti znamená, že používateľ nemá dostatočné oprávnenie na vykonanie požiadavky alebo že používateľ nemá licenciu na údaje, ku ktorých chce získať prístup. Úspešnú žiadosť môžu úspešne vykonať iba používatelia s požadovanými povoleniami alebo licenciami.

**403 Zakázané: Vybrali ste správne rozhranie API zdroja?**

Služby rozhrania API, ako je napríklad microsoft Graph, skontrolujte, či sa nárok aud (cieľová skupina) v prijatom prístupového tokene zhoduje s hodnotou, ktorú pre seba očakáva, a ak nie, výsledkom je chyba 403 Zakázané. Častou chybou, výsledkom ktorej je táto chyba, je pokus o použitie tokenu získaného pre rozhrania API Azure AD Graph, rozhrania API Outlooku alebo rozhrania API SharePointu/OneDrivu na volanie Microsoft Graph (alebo naopak). Uistite sa, že zdroj (alebo rozsah) vašej aplikácie získava token, ktorý sa zhoduje s rozhraním API, ktoré aplikácia volá.

**400 Nesprávna požiadavka alebo 403 Zakázané: Dodržiava používateľ politiky podmieneného prístupu svojej organizácie?**

Na základe politík certifikačnej autority organizácie môže byť používateľ, ktorý má prostredníctvom vašej aplikácie prístup k zdrojom spoločnosti Microsoft pre Graph, výzva na získanie ďalších informácií, ktoré sa v prístupového tokenu, ktorý vaša aplikácia pôvodne získala, nie sú. V tomto prípade sa v aplikácii zobrazí chyba 400 s chybou *interaction_required* (počas akvizície prístupového tokenu) alebo chyba 403 s chybou *insufficient_claims* (pri volaní do Microsoft Graph). V oboch prípadoch odpoveď na chybu obsahuje ďalšie informácie, ktoré môžu byť prezentované oprávneným koncovým bodom na výzvu pre používateľa, aby získal ďalšie informácie (napríklad viacfaktorové overovanie alebo registráciu zariadenia).

- [Riešenie problémov s podmieneným prístupom pomocou funkcie MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Pokyny pre vývojárov pre podmienený prístup k službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
