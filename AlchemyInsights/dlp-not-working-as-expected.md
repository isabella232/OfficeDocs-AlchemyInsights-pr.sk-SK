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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707825"
---
# <a name="dlp-not-working-as-expected"></a>DLP nefunguje podľa očakávania

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

 **Nastavenie DLP**

Vyskytli sa problémy s **prevenciou pred stratou údajov (DLP)** v Office 365 nefunguje podľa očakávania? Ak áno, uistite sa, že **politika DLP** je nastavená správne a že vaše údaje obsahujú informácie o tom, čo **politika DLP** hľadá pri jej vyhodnocovaní.
  
Politiky DLP vám umožňujú identifikovať a chrániť citlivé informácie vo vašej organizácii. Ak chcete nastaviť politiky DLP, použite informácie [tu](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).
  
 **Čo politiky DLP hľadajú**
  
Pri používaní **vstavaných typov citlivých informácií** v centre zabezpečenia a dodržiavania súladu majú politiky DLP pri zisťovaní týchto citlivých typov vyhľadať konkrétne vzory a prvky.
  
- **Vstavané typy citlivých informácií**

    Informácie o vstavaných citlivých typoch a o tom, čo politika DLP vyhľadáva pri zisťovaní citlivého typu, nájdete v téme: [Aké typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)vyhľadávajú.

- **Vlastné typy citlivých informácií**

    Ak sa pokúšate vytvoriť vlastné typy citlivých informácií, použite nasledujúci článok, kde nájdete informácie o tom, ako vytvoriť vlastný typ citlivosti: [Vytvorenie vlastného typu citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testovanie politiky DLP**

Ak chcete otestovať údaje pomocou vstavaného alebo vlastného typu citlivých informácií, použite možnosť **testovať typ** v časti **klasifikácie**  >  **citlivé typy informácií**. Ďalšie informácie nájdete v téme [testovanie vlastných typov citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Zostavy**
  
- Získajte podrobné informácie o citlivých údajoch so [zostavami DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Pozrite si konkrétne podrobnosti o udalosti s [hlásením incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
