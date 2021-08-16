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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069979"
---
# <a name="conditional-access-issues"></a>Problémy s podmieneným prístupom

**Riešenie problémov s diagnostikou prihlásenia**

Pomocou nástroja Diagnostika prihlásenia môžete rýchlo zistiť, čo sa stalo alebo diagnostikovať problémy súvisiace [s prihlásením používateľov:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Spustite nástroj Diagnostika prihlásenia.
1. Udalosť, ktorú chcete analyzovať, nájdete zadaním podrobností o používateľovi, aplikácii, čase prihlásenia, identifikácii požiadavky alebo identifikácii korelácie.
1. Skontrolujte diagnostické výsledky a pozrite si podrobnosti o tom, čo sa udialo, a aké akcie môžete vykonať pri ich zmenách (ak sú potrebné nejaké zmeny).

**Postup riešenia problémov s prihlásením** 

1. Prejdite na stránku prihlásenia do služby Azure AD.
1. Filtrujte prihlásenia podľa používateľa, časového rozsahu, aplikácie, stavu, klientskej aplikácie atď.
1. Vyberte udalosť prihlásenia a zobrazte kartu Podmienený prístup, aby ste videli, ktoré politiky boli vyhodnotené.
1. Kliknutím na riadok politiky zobrazte podrobnosti politiky a porozumiete jej dôvodom.

**Nástroje na riešenie problémov s politikou podmieneného prístupu**

- Režim iba zostava umožňuje vyhodnotiť politiku bez vplyvu na používateľov.
- Nástroj What-if vám umožňuje simulovať udalosti prihlásenia a zistiť, ktoré politiky sa majú použiť.
- Prehľady a vytváranie zostáv zošitov zobrazuje vplyv každej politiky v reálnom čase.

**Politiky ochrany podľa pôvodného plánu**

Politiky ochrany pôvodného plánu sa už nepoužívali. Už sa nebudú vynútiť a čoskoro sa odstránia z portálu Azure. Odporúčame povoliť [predvolené nastavenia zabezpečenia.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Ďalšie informácie o podmienenom prístupe nájdete v téme:

[Osvedčené postupy podmieneného prístupu v Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ovládacie prvky v podmienenom prístupe](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Umiestnenia v podmienenom prístupe](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
