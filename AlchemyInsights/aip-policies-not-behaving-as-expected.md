---
title: 'AIP: politiky sa nesprávajú podľa očakávaní'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663204"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: politiky sa nesprávajú podľa očakávaní

Azure ochrana informácií: politiky, ktoré sa nesprávajú podľa očakávaní, nájdete v téme Odporúčané pokyny pre rôzne politické problémy:

1. Ak máte problémy s vizuálnymi značkami, skontrolujte, či [sa používajú vizuálne označenia](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Ak máte problémy s automatickým označovaním, prečítajte [si tému Konfigurovanie podmienok pre automatickú a odporúčanú klasifikáciu na ochranu informácií Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a informácie o tom, [ktoré typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)vyhľadávajú.
3. Ak máte problémy s natívnou alebo Pfile ochranou, skontrolujte [konfiguráciu konfigurácie súboru API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Skontrolujte, či používate politiky rozsahu, ktoré nie sú správne nakonfigurované: [Konfigurácia politiky ochrany informácií Azure pre konkrétnych používateľov pomocou politiky rozsahu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ak automatické označenie nefunguje pre Outlook pri priložení označeného dokumentu, overte, či DRMEncryptProperty nie je definovaný, ako je to popísané nižšie: [nastavenia databázy Registry IRM pre zabezpečenie](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ak sa stále vyskytujú problémy, Zhromaždite denníky klienta Azure Information Protection a priložte exportované denníky do tejto letenky.

1. Otvorte dokument balíka Office alebo vytvorte nový e-mail v Outlooku.
2. Kliknite na položku **Ochrana**  >  **a citlivosť a pripomienky**.
3. Kliknite na položku **Exportovať denníky**.
4. Uložte denníky podľa vlastného výberu umiestnenia a priložte ich k tejto žiadosti o službu.

Ďalšie zdroje:

- [Konfigurácia označenia vizuálnych označení na ochranu informácií v službe Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Revízia dokumentácie služby Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Používanie označení citlivosti v aplikáciách Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

