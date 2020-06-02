---
title: DLP nefunguje podľa očakávania
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507493"
---
# <a name="dlp-not-working-as-expected"></a>DLP nefunguje podľa očakávania

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

 **Nastavenie DLP**

Máte problémy s **funkciou Ochrana pred únikom údajov (DLP)** v službách Office 365, ktoré nefungujú podľa očakávania? Ak áno, skontrolujte, či je **politika DLP** nastavená správne a či vaše údaje obsahujú to, čo **politika DLP** hľadá pri hodnotení.
  
Politiky DLP umožňujú identifikovať a chrániť citlivé informácie vo vašej organizácii. Ak chcete nastaviť politiky DLP, použite informácie [tu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Čo je to za politiky DLP**
  
Pri používaní **vstavaných typov citlivých informácií v** centrách zabezpečenia a dodržiavania súladu politiky DLP hľadajú pri zisťovaní týchto citlivých typov špecifické vzory a prvky.
  
- **Vstavané typy citlivých informácií**

    Informácie o vstavaných typoch citlivých údajov a o tom, čo politika DLP hľadá pri zisťovaní citlivého typu, nájdete v téme: [Čo vyzerajú typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Vlastné typy citlivých informácií**

    Ak sa pokúšate vytvoriť vlastné typy citlivých informácií, informácie o vytvorení vlastného typu citlivého obsahu: [Vytvorenie vlastného typu citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)použite nasledujúci článok.

**Testovanie politiky DLP**

Ak chcete otestovať údaje pomocou vstavaného alebo vlastného typu citlivých informácií, použite možnosť **Typ testu** v časti **Klasifikácie**  >  **Citlivé typy informácií**. Ďalšie informácie nájdete v téme [Testovanie vlastných typov citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Správy**
  
- Získajte prehľady citlivých údajov pomocou [zostáv DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Pozrite si konkrétne podrobnosti o udalosti so [správou o incidente](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
