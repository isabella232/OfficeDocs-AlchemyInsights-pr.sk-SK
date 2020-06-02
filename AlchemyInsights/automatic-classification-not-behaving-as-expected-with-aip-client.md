---
title: Automatická klasifikácia sa nespráva podľa očakávania s klientom AIP
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
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508391"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatická klasifikácia sa nespráva podľa očakávania s klientom AIP

Automatická klasifikácia sa nespráva podľa očakávania, použite nasledujúce odporúčané pokyny:

1. Ak máte problémy s automatickým označovaním, pozrite si tému [Konfigurácia podmienok automatickej a odporúčanej klasifikácie služby Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) a možnosti vyhľadávania typov [citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Skontrolujte, či používate politiky rozsahu, ktoré nie sú správne nakonfigurované: [Ako nakonfigurovať politiku Azure ochranu informácií pre konkrétnych používateľov pomocou politiky rozsahu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Ak automatické označovanie nefunguje pre program Outlook pri pripájaní označeného dokumentu, overte, či `DRMEncryptProperty` nie je definovaný podľa popisu: Nastavenie [databázy Registry správy prístupových práv k informáciám pre zabezpečenie](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ak ste pre politiku ochrany informácií azure použili [vstavané typy informácií,](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) overte, či sa váš obsah zhoduje s očakávaným formátom.
5. Skontrolujte, či je menovka vhodne nakonfigurovaná pre **automatické** alebo **odporúčané**. **(Automatické** označovanie je k dispozícii pre všetky aplikácie balíka Office, zatiaľ čo **odporúčané** je k dispozícii pre všetky aplikácie balíka Office okrem Outlooku.)
6. Nemôžete použiť automatickú klasifikáciu pre dokumenty a e-maily, ktoré boli predtým manuálne označené alebo predtým automaticky označené vyššou klasifikáciou.  Ďalšie informácie nájdete v téme: [Ako sa používajú automatické alebo odporúčané menovky](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Ak ste stále problémy, zbierajte Azure informácie ochrany denníky klienta a pripojiť exportované denníky na lístok technickej podpory. Exportovanie denníkov Azure information protection:
    - Otvorte dokument balíka Office alebo vytvorte nový e-mail v programe Outlook.
    - Kliknite na **položku Pomôcť a spätnú**väzbu o ochrane  >  **a citlivosti**.
    - Kliknite na **položku Exportovať denníky**.
    - Uložte denníky podľa vášho výberu miesta a pripojte ich k žiadosti o službu.

Ďalšie informácie nájdete v témach:

- [Ako nakonfigurovať podmienky pre automatické a odporúčané klasifikácie Azure informácie ochrany](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Príručky pre bežné scenáre, ktoré používajú službu Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Preskúmanie dokumentácie azure information protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Kontrola predplatných a funkcií služby Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Požiadavky na ochranu informácií azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Kurz rýchleho spustenia pre službu Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Stiahnuť Azure informácie ochrany klienta](https://www.microsoft.com/download/details.aspx?id=53018)
