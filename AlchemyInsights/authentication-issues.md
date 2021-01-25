---
title: Problémy s overovaním
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
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974792"
---
# <a name="authentication-issues"></a>Problémy s overovaním

**Hľadáte informácie o chybových kódoch AADSTS, ktoré sa vracajú zo služby tokenu zabezpečenia služby Azure Active Directory (Azure AD) (STS)?** Pozrite si tému [kódy chýb overovania služby Azure AD a povolenie](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) na vyhľadanie AADSTS chýb, opráv a niektorých navrhovaných alternatívnych riešení.

Chyby autorizácie môžu byť výsledkom niekoľkých rôznych problémov, z ktorých väčšina vygeneruje chybu 401 alebo 403. Nasledujúce problémy môžu viesť k chybám autorizácie:

- Nesprávny [tok získavania tokenov prístupu](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Nesprávne nakonfigurované [rozsahy povolení](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Nedostatok [súhlasu](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Ak chcete vyriešiť bežné chyby autorizácie, vyskúšajte nižšie uvedené kroky, ktoré sa najviac zhodujú s chybou, ktorú dostávate. Pri prijatí chyby môže platiť viac ako jeden krok.

- **401 Nepovolená chyba: je token platný?**

Uistite sa, že vaša aplikácia prezentuje platný prístupový token programu Microsoft Graph ako súčasť žiadosti. Táto chyba často znamená, že prístupový token môže chýbať v hlavičke žiadosti o overenie HTTP alebo že token je neplatný alebo uplynul. Dôrazne odporúčame, aby ste používali Microsoft Authentication Library (MSAL) na získanie prístupových tokenov. Táto chyba sa môže vyskytnúť aj vtedy, keď sa pokúsite použiť delegovaný prístupový token poskytnutý na osobné konto Microsoft na prístup k API, ktoré podporuje iba pracovné alebo školské kontá (organizačné kontá).

**403 zakázaná chyba: vybrali ste správnu množinu povolení?**

Uistite sa, že ste požiadali o správnu množinu povolení na základe API aplikácie Microsoft Graph, ktoré vaše hovory z aplikácií používajú. Odporúčané minimálne privilegované povolenia sú k dispozícii vo všetkých témach o referenčnej metóde rozhrania Microsoft Graph API. Okrem toho musia tieto povolenia udeliť používateľovi alebo správcovi žiadosť. Udelenie povolení sa zvyčajne uskutočňuje prostredníctvom stránky súhlasu alebo používania čepele na registráciu aplikácie Azure Portal. V časti **Nastavenie** kotúča pre aplikáciu kliknite na položku **požadované povolenia** a potom kliknite na položku **udeliť povolenia**. Ďalšie informácie nájdete v téme:

- [Povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Informácie o povoleniach a súhlasu v službe Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 zakázaná chyba: zistilo sa, že vaša aplikácia získala token, aby zodpovedal vybraným povoleniam?**

Presvedčte sa, že typy požadovaných povolení alebo udelené povolenia sa zhodujú s typom accessového tokenu, ktorý vaša aplikácia nadobudne. Môže sa stať, že požadujete a udelíte povolenia aplikácie, ale použijete tokeny na tok delegovaných interaktívnych kódov namiesto tokenov toku klientskych poverení, alebo požadujete a udelíte delegované povolenia, ale použijete tokeny toku klientskych poverení namiesto použitia tokenov toku delegovaných kódov.

Ďalšie informácie týkajúce sa získavania tokenov nájdete v témach:

- [Získanie prístupu v mene používateľov a delegovaných povolení](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0 – OAuth 2,0 autorizačný kód](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Získanie prístupu bez používateľa (služba daemon) a povolenia aplikácie](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0 – OAuth 2,0 klientsky tok poverení](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 zakázaná chyba: obnovenie hesla**

Momentálne nie sú k dispozícii žiadne povolenia na používanie služby daemon Service – to-Service, ktoré umožňujú obnovenie používateľských hesiel. Tieto rozhrania API sú podporované iba pomocou interaktívneho delegovaného kódu s prihláseným správcom. Ďalšie informácie nájdete v téme [povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 zakázané: má používateľ prístup a je im licencovaný?**

V prípade tokov delegovaných kódov Microsoft Graph vyhodnotí, či bola požiadavka povolená na základe povolení udelených pre aplikáciu a povolení, ktoré má používateľ s prihlásením. Vo všeobecnosti platí, že táto chyba znamená, že používateľ nie je dostatočne privilegovaný na vykonanie žiadosti **alebo** Ak používateľ nemá licenciu na údaje, ktoré sú k dispozícii. Žiadosť môže úspešne vykonať len používateľ s požadovanými povoleniami alebo licenciami.

**403 zakázané: vybrali ste správne rozhranie API zdroja?**

Služby API, ako je napríklad Microsoft Graph, skontrolujte, či sa nárok na *AUD* (Cieľová skupina) v prijatom accessovom tokene zhoduje s hodnotou, ktorú očakáva sám, a ak nie, vyskytne sa chyba 403 Forbidden. Bežnou chybou, ktorá má za následok túto chybu, sa pokúša použiť token získaný pre rozhrania API služby Azure AD Graph, rozhrania API programu Outlook alebo služby SharePoint/OneDrive na volanie do programu Microsoft Graph (alebo naopak). Uistite sa, že zdroj (alebo rozsah) vašej aplikácie získava token pre zhodu rozhrania API, ktoré aplikácia volá.

**400 Nesprávna žiadosť alebo 403 je zakázaná: používateľ dodržiava politiky podmieneného prístupu svojej organizácie (CA)?**

Na základe politík podmieneného prístupu organizácie môže používateľ, ktorý získava prístup k zdrojom Microsoft Graphu prostredníctvom vašej aplikácie, spochybniť ďalšie informácie, ktoré sa nenachádzajú v accessovom tokene, v ktorom bola vaša aplikácia pôvodne získaná. V tomto prípade aplikácia dostane **400 s chybou *interaction_required*** pri získavaní tokenu prístupu alebo **403 s *Insufficient_claimsou*** chybou pri volaní Microsoft Graphu. V obidvoch prípadoch obsahuje odpoveď na chyby Ďalšie informácie, ktoré možno predložiť oprávnenému koncovému bodu, aby napadli používateľovi ďalšie informácie (napríklad overovanie viacerých faktorov alebo registrácia zariadenia).

Ďalšie informácie týkajúce sa podmieneného prístupu nájdete v témach:

- [Riešenie problémov s podmieneným prístupom pomocou MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Usmernenie vývojára pre podmienený prístup k službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Koniec podpory pre Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph)_* _

- Od 30. júna 2020, už nebudeme pridávať žiadne nové funkcie do služby Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph). Budeme aj naďalej poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudú poskytovať aktualizácie funkcií.
- Od 30. júna 2022, ukončíme podporu pre ADAL a AAD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia.
    - Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však mať žiadne technické podpory ani aktualizácie zabezpečenia.
    - Aplikácie, ktoré používajú AAD Graph po uplynutí tohto času, už nemusia dostávať odpovede od koncového bodu v grafe AAD.

_ *Migrácia ADAL**

Odporúčame aktualizovať na [knižnicu Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ktorá obsahuje najnovšie funkcie a aktualizácie zabezpečenia. Toto odporúčanie je v kontexte Microsoft migrácia svojich aplikácií na MSAL podľa termínu ukončenia podpory. Cieľom migrácie aplikácií od spoločnosti Microsoft k MSAL je zabezpečiť, aby aplikácie profitovali z pokračujúcich vylepšení zabezpečenia a funkcií MSAL.

- [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Informácie o tom, ako migrovať aplikácie na základe jednotlivých platforiem](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ak potrebujete pomoc s pochopením, ktoré z vašich aplikácií používajú ADAL, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a v prípade potreby osloviť nezávislých dodávateľov softvéru (ISV) alebo poskytovateľov aplikácií. Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií, ktoré nie sú Microsoft ADAL v nájomníkovi.

**Migrácia grafu AAD**

V prípade aplikácií, ktoré používajú AAD Graph, postupujte podľa pokynov na [migráciu aplikácií služby Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Náš kontrolný zoznam migrácie poskytuje bod začiatku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Na portáli registrácie aplikácie Azure sa zobrazuje, ktoré aplikácie používajú AAD Graph. Odporúčame, aby ste si prečítali všetky zdrojové kódy aplikácií a ak je to možné, Oslovte ľubovoľných poskytovateľov ISV alebo aplikácií. Technická podpora spoločnosti Microsoft vám tiež poskytuje informácie o všetkých použitiach AAD grafov v nájomníkovi.

 










