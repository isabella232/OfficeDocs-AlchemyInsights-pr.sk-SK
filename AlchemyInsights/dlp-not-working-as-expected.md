---
title: DLP nefunguje podľa očakávania
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079717"
---
# <a name="dlp-not-working-as-expected"></a>DLP nefunguje podľa očakávania

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

 **Nastavenie DLP**

Máte problémy s **stratou údajov (DLP) v** prípade, Office 365 nefunguje podľa očakávaní? Ak áno, skontrolujte, či je politika **DLP** nastavená správne a či vaše údaje obsahujú to, čo hľadá politika **DLP** pri vyhodnocovaní.
  
Politiky DLP vám umožňujú identifikovať a chrániť citlivé informácie vo vašej organizácii. Ak chcete nastaviť politiky DLP, použite informácie [uvedené tu.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Čo sa v politikách DLP vyhľadá**
  
Pri používaní **vstavaných typov citlivých** informácií v centrách zabezpečenia a dodržiavania súladu sa v rámci politík DLP pri zisťovaní týchto citlivých typov budú hľadať konkrétne vzory a prvky.
  
- **Vstavané typy citlivých informácií**

    Informácie o vstavaných typoch Citlivé a o tom, čo sa hľadá v rámci politiky DLP pri zisťovaní typu Citlivé, nájdete v téme: Čo vyhľadávajú typy [citlivých informácií.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Vlastné typy citlivých informácií**

    Ak sa pokúšate vytvoriť vlastné typy citlivých informácií, v nasledujúcom článku nájdete informácie o tom, ako vytvoriť vlastný citlivý typ: Vytvorenie vlastného typu [citlivých informácií.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Testovanie politiky DLP**

Ak chcete údaje otestovať pomocou vstavaného alebo vlastného typu citlivých informácií, použite **možnosť Typ testu** v časti **Klasifikácie**  >  **Typy citlivých informácií.** Ďalšie informácie nájdete v téme [Testovanie vlastných typov citlivých informácií.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Zostavy**
  
- Získajte prehľad o citlivých údajoch pomocou [zostáv DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Pozrite si konkrétne podrobnosti udalosti so správou [o incidente.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
