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
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934308"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Politiky sa nesprávajú podľa očakávania

Azure Information Protection: Politiky sa nesprávajú podľa očakávaní, v nasledujúcich odporúčaných pokynoch pre rôzne problémy s politikami:

1. Ak máte problémy so vizuálnymi označeniami, pozrite si [položku Pri použití vizuálnych označení.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ak máte problémy s automatickým označením, pozrite si témy Konfigurácia podmienok pre automatickú a odporúčanú klasifikáciu služby [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a Čo hľadia typy [citlivých informácií.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Ak máte problémy s ochranou natívneho súboru alebo súboru Pfile, pozrite si [konfiguráciu rozhrania API súboru.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Skontrolujte, či používate politiky rozsahov, ktoré nie sú správne [nakonfigurované:](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)Konfigurácia politiky Azure Information Protection pre konkrétnych používateľov pomocou politík s rozsahom .
5. Ak automatické označovanie nefunguje pre Outlook pri priložení označeného dokumentu, overte, či nie je možnosť DRMEncryptProperty definovaná takto: Nastavenie IRM databázy [Registry pre zabezpečenie.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Ak problémy aj naďalej pretrváva, zhromaždite denníky klientov Azure Information Protection a priložte exportované denníky k tejto lístku.

1. Otvorte dokument Office alebo vytvorte nový e-mail v Outlook.
2. Kliknite **na položku Pomocník a pripomienky k ochrane** alebo  >  **citlivosti.**
3. Kliknite na **položku Exportovať denníky**.
4. Uložte denníky podľa vášho výberu a priložte ich k tejto žiadosti o službu.

Ďalšie zdroje:

- [Konfigurácia označenia pre vizuálne označenia pre Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Kontrola dokumentácie služby Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Použitie označení citlivosti v Microsoft 365 aplikáciách](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

