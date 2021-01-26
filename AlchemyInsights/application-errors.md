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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984659"
---
# <a name="application-errors"></a>Chyby aplikácie

Hľadáte informácie o **chybových kódoch AADSTS** , ktoré sa vracajú zo služby tokenu zabezpečenia služby Azure Active Directory (Azure AD) (STS)? Prečítajte si [kódy chýb overovania Azure AD a povolenie](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) na nájdenie AADSTS chýb, opráv a niektorých navrhovaných alternatívnych riešení.

Chyby autorizácie môžu byť výsledkom niekoľkých rôznych problémov, z ktorých väčšina vygeneruje chybu 401 alebo 403. Tieto chyby môžu viesť napríklad k chybám autorizácie:

- Nesprávny [tok získavania tokenov prístupu](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Nesprávne nakonfigurované [rozsahy povolení](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Nedostatok [súhlasu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Ak chcete vyriešiť bežné chyby autorizácie, vyskúšajte nižšie uvedené kroky, ktoré sa najviac zhodujú s chybou, ktorú dostávate. Môže sa použiť viac ako jeden.

**401 Nepovolená chyba: je token platný?**

Uistite sa, že vaša aplikácia prezentuje platný prístupový token programu Microsoft Graph ako súčasť žiadosti. Táto chyba často znamená, že prístupový token môže chýbať v hlavičke žiadosti o overenie HTTP alebo že token je neplatný alebo uplynul. Dôrazne odporúčame, aby ste používali [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) na získanie prístupových tokenov. Okrem toho táto chyba sa môže vyskytnúť, ak sa pokúsite použiť delegovaný prístupový token poskytnutý na osobné konto Microsoft na prístup k API, ktoré podporuje iba pracovné alebo školské kontá (kontá organizácie).

**403 zakázaná chyba: vybrali ste správnu množinu povolení?**

Skontrolujte, či ste požiadali o správnu množinu povolení na základe API aplikácie Microsoft Graph, ktoré vaše hovory z aplikácií používajú. Odporúčané minimálne privilegované povolenia sú k dispozícii vo všetkých témach o referenčnej metóde rozhrania Microsoft Graph API. Okrem toho musia tieto povolenia udeliť používateľovi alebo správcovi žiadosť. Udelenie povolení sa zvyčajne uskutočňuje prostredníctvom stránky súhlasu alebo poskytnutím povolení pomocou funkcie na registráciu aplikácie Azure Portal. V časti **Nastavenie** kotúča pre aplikáciu kliknite na položku **požadované povolenia** a potom kliknite na položku **udeliť povolenia**.

- [Povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Informácie o povoleniach a súhlasu v službe Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 zakázaná chyba: zistilo sa, že vaša aplikácia získala token, aby zodpovedal vybraným povoleniam?**

Uistite sa, že požadovaný typ povolení alebo udelenie sa zhoduje s typom accessového tokenu, ktorý vaša aplikácia nadobudne. Môže sa stať, že požadujete a udelíte povolenia na používanie, ale použijete tokeny na tok delegovaných interaktívnych kódov namiesto tokenov toku klientskych poverení, alebo požadujete a udelíte delegované povolenia, ale použijete tokeny toku klientskych poverení namiesto prispôsobených tokenov.

- [Získanie prístupu v mene používateľov a delegovaných povolení](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0 – OAuth 2,0 autorizačný kód](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Získanie prístupu bez používateľa (služba daemon) a povolenia aplikácie](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0 – OAuth 2,0 klientsky tok poverení](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 zakázaná chyba: obnovenie hesla**

Momentálne nie sú k dispozícii žiadne povolenia na používanie služby daemon Service – to-Service, ktoré umožňujú obnovenie používateľských hesiel. Tieto rozhrania API sú podporované iba pomocou interaktívneho delegovaného kódu s prihláseným správcom.

- [Povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 zakázané: má používateľ prístup a je im licencovaný?**

V prípade tokov delegovaných kódov sa v programe Microsoft Graph vyhodnotí, či je žiadosť povolená na základe povolení udelených pre aplikáciu a povolení, ktoré má používateľ s prihlásením. Vo všeobecnosti platí, že táto chyba znamená, že používateľ nie je dostatočne privilegovaný na vykonanie žiadosti alebo ak používateľ nemá licenciu na údaje, ktoré sú k dispozícii. Žiadosť môže úspešne vykonať len používateľ s požadovanými povoleniami alebo licenciami.

**403 zakázané: vybrali ste správne rozhranie API zdroja?**

Služby API, ako je napríklad Microsoft Graph, skontrolujte, či sa nárok na AUD (Cieľová skupina) v prijatom accessovom tokene zhoduje s hodnotou, ktorú očakáva sám, a ak nie, výsledkom je zakázaná chyba 403. Bežnou chybou, ktorá má za následok túto chybu, sa pokúša použiť token získaný pre rozhrania API služby Azure AD Graph, rozhrania API programu Outlook alebo služby SharePoint/OneDrive na volanie do programu Microsoft Graph (alebo naopak). Uistite sa, že zdroj (alebo rozsah) vašej aplikácie získava token pre zhodu rozhrania API, ktoré aplikácia volá.

**400 Nesprávna žiadosť alebo 403 je zakázaná: používateľ dodržiava politiky podmieneného prístupu svojej organizácie (CA)?**

Na základe politík certifikačnej autority organizácie môže používateľ, ktorý získava prístup k zdrojom Microsoft Graphu prostredníctvom vašej aplikácie, spochybniť ďalšie informácie, ktoré sa nenachádzajú v accessovom tokene, v ktorom bola vaša aplikácia pôvodne získaná. V tomto prípade aplikácia dostane 400 s chybou *interaction_required* pri získavaní tokenu prístupu alebo 403 s *insufficient_claimsou* chybou pri volaní Microsoft Graphu. V obidvoch prípadoch obsahuje odpoveď na chyby Ďalšie informácie, ktoré môžu byť prezentované na koncovom bode autorizácie, aby napadli používateľovi ďalšie informácie (napríklad overovanie viacerých faktorov alebo registrácia zariadenia).

- [Riešenie problémov s podmieneným prístupom pomocou MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Usmernenie vývojára pre podmienený prístup k službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
