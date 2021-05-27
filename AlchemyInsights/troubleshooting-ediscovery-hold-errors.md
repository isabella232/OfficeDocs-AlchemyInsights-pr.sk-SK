---
title: Riešenie chýb blokovania ediscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676282"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Riešenie chýb blokovania ediscovery

Vyskytli sa problémy s blokovania eDiscovery? Tu je niekoľko najvhodnejších postupov na zváženie:

- Skontrolujte stav zadržanej distribúcie.  Ak je stav **On (Pending) alebo Off** **(Pending) (Nevybavené),** počkajte, kým sa distribúcia zadržaho dokončí.
- Zlúčenie vyhľadávania eDiscovery – zadržanie aktualizácií do jednej hromadnej požiadavky namiesto opakovaného aktualizovania politiky pre každú transakciu.
- V Set-CaseHoldPolicy <policyname> Powershell Centra zabezpečenia a dodržiavania súladu spustite príkaz -RetryDistribution. Podrobnosti nájdete v téme [Pripojenie zabezpečenia & Compliance Center PowerShell.](/powershell/exchange/connect-to-scc-powershell)

Kroky na kontrolu týchto nastavení a ďalšie osvedčené postupy na riešenie problémov s riešením blokovania eDiscovery nájdete v téme Riešenie chýb blokovania [eDiscovery.](/microsoft-365/compliance/hold-distribution-errors)
Informácie o riešení iných bežných problémov s eDiscovery nájdete v téme [Skúmanie, riešenie a riešenie bežných problémov s eDiscovery.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
