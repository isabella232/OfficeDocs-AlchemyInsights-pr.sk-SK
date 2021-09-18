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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446706"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP možno bude potrebovať vlastný typ

**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).

**DLP môže vyžadovať vlastný typ informácií**

Pomocou politiky ochrany pred stratou údajov (DLP) môžete identifikovať a chrániť citlivé údaje vo svojej organizácii. V niektorých situáciách môže byť potrebné vytvoriť vlastný typ citlivých informácií na ochranu údajov vašej organizácie. Ďalšie informácie nájdete v téme Informácie [o typoch citlivých informácií a](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) definíciách [entít typu Citlivé informácie.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Ďalšie informácie o vytváraní vlastných typov a politík citlivých informácií nájdete v téme: 

**Prispôsobenie vstavaného typu citlivých informácií**

Ak by vám vstavaný typ citlivých informácií vyhovoval vašim potrebám pomocou niekoľkých úprav, pozrite si časť Prispôsobenie vstavaného [typu citlivých informácií.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Môžete napríklad pridať alebo odstrániť kľúčové slová alebo pridať alebo odstrániť podporné dôkazy, ako je napríklad dátum alebo adresa.

**Vytvorenie vlastného typu citlivých informácií**

Ak však potrebujete identifikovať a chrániť iný typ citlivých informácií, môžete v texte vytvoriť vlastný typ citlivých informácií Centrum dodržiavania súladu pre Microsoft 365. Ďalšie informácie nájdete v téme [Začíname s vlastnými typmi citlivých informácií.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Vytvorenie vlastného typu citlivých informácií v prostredí & Compliance Center PowerShell**

Ak používateľské rozhranie neposkytuje všetky potrebné možnosti, môžete v prostredí PowerShell centra zabezpečenia a dodržiavania & informácií vytvoriť vlastný typ citlivých informácií. Po spustení súboru XML môžete použiť všetky dostupné možnosti. Ďalšie informácie nájdete v téme [Vytvorenie typu vlastných citlivých informácií pomocou prostredia PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Ak chcete najprv otestovať politiku v testovacom režime, pozrite si téme Implementácia politiky v [testovacom](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) režime [a Vytvorenie, testovanie a ladenie politiky DLP.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 