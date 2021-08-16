---
title: DLP možno bude potrebovať vlastný typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030809"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP možno bude potrebovať vlastný typ

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**DLP môže vyžadovať vlastný typ informácií**

Pomocou politiky ochrany pred stratou údajov (DLP) môžete identifikovať a chrániť citlivé údaje vo svojej organizácii. V niektorých situáciách môže byť potrebné vytvoriť vlastný **typ** citlivých informácií na ochranu údajov vašej organizácie.

Vaša organizácia môže napríklad potrebovať identifikovať a chrániť IDENTIFIKÁCIE zamestnancov alebo iné údaje v inom formáte, ktorý je špecifický pre vašu organizáciu. Ak áno, pozrite si ďalšie informácie v nasledujúcich článkoch.
  
 **Prispôsobenie vstavaného typu citlivých informácií**
  
Ak by vám vstavaný typ citlivých informácií vyhovoval vašim potrebám pomocou niekoľkých úprav, môžete prispôsobiť vstavaný [typ citlivých informácií.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Môžete napríklad pridať alebo odstrániť kľúčové slová alebo pridať alebo odstrániť podporné dôkazy, ako je napríklad dátum alebo adresa.
  
 **Vytvorenie vlastného typu citlivých informácií**
  
Ak však potrebujete identifikovať a chrániť úplne iný typ citlivých informácií, môžete v používateľskom rozhraní Centra zabezpečenia [a](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) dodržiavania súladu vytvoriť vlastný typ & citlivých informácií.
  
**Vytvorenie vlastného typu citlivých informácií v prostredí & Compliance Center PowerShell**

Ak používateľské rozhranie neposkytne všetky potrebné možnosti, môžete v prostredí [Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)vytvoriť vlastný typ citlivých informácií. Po spustení súboru XML môžete použiť všetky dostupné možnosti.
