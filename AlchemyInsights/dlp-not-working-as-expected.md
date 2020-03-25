---
title: DLP nefunguje podľa očakávania
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932637"
---
# <a name="dlp-not-working-as-expected"></a>DLP nefunguje podľa očakávania

**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí. Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania. Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.

Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa. Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch. Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.

 **Nastavenie DLP**

Máte problémy s **únikom údajov (DLP)** v balíku Office 365 nefunguje podľa očakávania? Ak áno, uistite sa, že **DLP politika** je nastavená správne, a že vaše údaje obsahuje to, čo **DLP politika** hľadá, keď sa hodnotí.
  
Politiky DLP vám umožňujú identifikovať a chrániť citlivé informácie vo vašej organizácii. Ak chcete nastaviť politiky DLP, použite informácie [tu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Čo DLP politiky Hľadať**
  
Pri použití **vstavané typy citlivých informácií** v Office 365 zabezpečenia a súladu centrum, DLP politiky Hľadať špecifické vzory a prvky pri zisťovaní týchto citlivých typov.
  
- **Vstavané typy citlivých informácií**

    Informácie o vstavaných citlivých typoch a o tom, čo politika DLP vyhľadáva pri zisťovaní citlivého typu, nájdete v téme: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Vlastné citlivé typy informácií**

    Ak sa pokúšate vytvoriť vlastné citlivé typy informácií, použite nasledujúci článok informácie o tom, ako vytvoriť vlastný citlivý typ: [vytvoriť vlastné citlivé informácie typu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Testovanie politiky DLP**

Ak chcete otestovať údaje pomocou vstavaného alebo vlastného typu citlivých informácií, použite možnosť **typ testu** podľa **klasifikácie** > **citlivých typov**informácií. Ďalšie informácie nájdete v téme [testovanie vlastných typov citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Správy**
  
- Získajte citlivé údaje s [prehľadom DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Pozrite si konkrétne podrobnosti udalosti so [správou o incidente](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
