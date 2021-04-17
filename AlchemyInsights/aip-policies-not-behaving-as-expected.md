---
title: 'AIP: Politiky sa nesprávajú podľa očakávania'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821642"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politiky sa nesprávajú podľa očakávania

Azure Information Protection: Politiky sa nesprávajú podľa očakávaní, v nasledujúcich odporúčaných pokynoch pre rôzne problémy s politikami:

1. Ak máte problémy so vizuálnymi označeniami, pozrite si [položku Pri použití vizuálnych označení.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ak máte problémy s automatickým označením, pozrite si témy Konfigurácia podmienok pre automatickú a odporúčanú klasifikáciu služby [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a Čo hľadia typy [citlivých informácií.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Ak máte problémy s ochranou natívneho súboru alebo súboru Pfile, pozrite si [konfiguráciu rozhrania API súboru.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Skontrolujte, či používate politiky rozsahov, ktoré nie sú správne [nakonfigurované:](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)Konfigurácia politiky Azure Information Protection pre konkrétnych používateľov pomocou politík s rozsahom .
5. Ak automatické označovanie nefunguje pre Outlook pri priložení označeného dokumentu, overte, či nie je možnosť DRMEncryptProperty definovaná podľa popisu v tomto článku: Nastavenia IRM databázy [Registry pre zabezpečenie.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Ak problémy aj naďalej pretrváva, zhromaždite denníky klientov Azure Information Protection a priložte exportované denníky k tejto lístku.

1. Otvorte dokument balíka Office alebo vytvorte nový e-mail v Outlooku.
2. Kliknite **na položku Pomocník a pripomienky k ochrane** alebo  >  **citlivosti.**
3. Kliknite na **položku Exportovať denníky**.
4. Uložte denníky podľa vášho výberu a priložte ich k tejto žiadosti o službu.

Ďalšie zdroje:

- [Konfigurácia označenia pre vizuálne označenia pre Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Kontrola dokumentácie služby Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Použitie označení citlivosti v aplikáciách služby Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

