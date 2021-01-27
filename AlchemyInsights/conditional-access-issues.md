---
title: Problémy s podmieneným prístupom
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
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015000"
---
# <a name="conditional-access-issues"></a>Problémy s podmieneným prístupom

**Riešenie problémov s diagnostickým prihlasovaním**

Pomocou [diagnostiky prihlásenia](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)môžete rýchlo zistiť, čo sa stalo alebo diagnostikovať problémy súvisiace s prihlasovaním používateľa:

1. Spustite diagnostické prihlásenie.
1. Nájdite udalosť, ktorú chcete analyzovať, zadaním podrobností o používateľovi, aplikácii, čase prihlásenia, ID požiadavky alebo identifikácii korelácie.
1. Prezrite si výsledky diagnostiky zobrazujúce Podrobnosti o tom, čo sa stalo a aké akcie môžete vykonať na vykonanie zmien (ak sú potrebné nejaké zmeny).

**Postup pri riešení problémov s prihlásením** 

1. Prejdite na prihlasovaciu stránku služby Azure AD.
1. Filtrovanie prihlasovacích hodnôt podľa používateľov, časového rozsahu, aplikácie, stavu, klientskej aplikácie atď.
1. Vyberte udalosť prihlásenia a zobrazte kartu podmieneného prístupu a zistite, ktoré politiky boli vyhodnotené.
1. Kliknutím na riadok politiky zobrazíte Podrobnosti o politike a rozumiete, prečo sa používa.

**Nástroje na riešenie politiky podmieneného prístupu**

- Režim iba zostavy vám umožňuje vyhodnotiť politiku bez ovplyvnenia používateľov.
- Nástroj co-If vám umožní simulovať udalosti pri prihlasovaní a zistiť, ktoré politiky sa používajú.
- V zošite s prehľadmi a správami sa zobrazuje vplyv každej politiky v reálnom čase.

**Politiky ochrany podľa pôvodného plánu**

Politiky ochrany podľa pôvodného plánu boli zastarané. Už nie sú presadzované a čoskoro sa odstránia z portálu Azure. Odporúčame povoliť [predvolené nastavenia zabezpečenia](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Ďalšie informácie o podmienenom prístupe nájdete v téme:

[Najvhodnejšie postupy pri podmienenom prístupe v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Podmienky v podmienenom prístupe](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ovládacie prvky v podmienenom prístupe](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Umiestnenia v podmienenom prístupe](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
