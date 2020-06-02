---
title: 'AIP: Politiky sa nesprávajú podľa očakávania'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493417"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politiky sa nesprávajú podľa očakávania

Azure informácie ochrana: Politiky sa nesprávajú podľa očakávania, nájdete v nasledujúcich častiach odporúčané pokyny pre rôzne problémy s politikou:

1. Ak máte problémy s vizuálnymi označeniami, prečítajte si článok [Pri použití vizuálnych označení](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Ak máte problémy s automatickým označovaním, prečítajte si tému [Konfigurácia podmienok pre automatickú a odporúčanú klasifikáciu služby Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a o [tom, čo citlivé typy informácií hľadajú.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
3. Ak máte problémy s natívnou ochranou/pfile, prečítajte si [konfiguráciu rozhrania API súboru](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Skontrolujte, či používate politiky rozsahu, ktoré nie sú správne nakonfigurované: [Ako nakonfigurovať politiku Azure ochranu informácií pre konkrétnych používateľov pomocou politiky rozsahu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ak automatické označovanie nefunguje pre program Outlook pri pripájaní označeného dokumentu, overte, či vlastnosť DRMEncryptProperty nie je definovaná podľa popisu: [Nastavenie databázy Registry správy prístupových práv k informáciám pre zabezpečenie](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ak problémy pretrvávajú, zhromažďovať Denníky klienta Azure information protection a pripojiť exportované denníky k tejto letenke.

1. Otvorte dokument balíka Office alebo vytvorte nový e-mail v programe Outlook.
2. Kliknite na **položku Pomôcť a spätnú**väzbu o ochrane  >  **a citlivosti**.
3. Kliknite na **položku Exportovať denníky**.
4. Uložte denníky podľa vášho výberu miesta a pripojte ich k tejto žiadosti o službu.

Ďalšie zdroje:

- [Ako nakonfigurovať označenie pre vizuálne značenie Azure informácie ochrany](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Preskúmanie dokumentácie azure information protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Používanie menoviek citlivosti v aplikáciách balíka Office](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

