---
title: Pri klientovi AIP sa automatická klasifikácia nespráva podľa očakávaní
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
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820913"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Pri klientovi AIP sa automatická klasifikácia nespráva podľa očakávaní

Automatická klasifikácia sa nespráva podľa očakávaní, použite tieto odporúčané pokyny:

1. Ak máte problémy s automatickým označením, pozrite si témy Konfigurácia podmienok pre automatickú a odporúčanú klasifikáciu pre [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a Čo sa v typoch citlivých informácií [hľadali.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Skontrolujte, či používate politiky rozsahov, ktoré nie sú správne [nakonfigurované:](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)Konfigurácia politiky Azure Information Protection pre konkrétnych používateľov pomocou politík s rozsahom .
3. Ak pri pripájaní označeného dokumentu nefunguje automatické označovanie pre Outlook, overte, či nie je definovaný podľa popisu nižšie: Nastavenia `DRMEncryptProperty` [IRM databázy Registry pre zabezpečenie.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Ak ste pre politiku Azure Information Protection [použili](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) vstavané typy informácií, overte, či sa obsah zhoduje s očakávaným formátom.
5. Overte, či je označenie správne nakonfigurované pre **možnosť Automaticky alebo** **Odporúčané.** (**Automatické označovanie** je k dispozícii pre všetky aplikácie microsoft 365, **zatiaľ** čo odporúčané je k dispozícii pre všetky aplikácie Microsoft 365 okrem Outlooku.)
6. Automatickú klasifikáciu nie je možné použiť pre dokumenty a e-maily, ktoré boli predtým manuálne označené alebo predtým automaticky označené vyššou klasifikáciou.  Ďalšie informácie nájdete v téme: [Použitie automatických alebo odporúčaných označení.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Ak problémy aj naďalej pretrváva, zhromaždite denníky klientov Azure Information Protection a priložte exportované denníky k lístku technickej podpory. Exportovanie denníkov Azure Information Protection:
    - Otvorte dokument balíka Office alebo vytvorte nový e-mail v Outlooku.
    - Kliknite **na položku Pomocník a pripomienky k ochrane** alebo  >  **citlivosti.**
    - Kliknite na **položku Exportovať denníky**.
    - Uložte denníky podľa vášho výberu a priložte ich k žiadosti o službu.

Ďalšie informácie nájdete v téme:

- [Postup konfigurácie podmienok pre automatickú a odporúčanú klasifikáciu pre Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Príručky s návodmi pre bežné scenáre, ktoré používajú Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Kontrola dokumentácie služby Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Kontrola predplatných a funkcií služby Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Požiadavky na službu Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Kurz so stručným návodom pre Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Stiahnutie klienta Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
