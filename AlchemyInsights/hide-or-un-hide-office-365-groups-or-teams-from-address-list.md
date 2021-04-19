---
title: Skrytie alebo zrušenie skrytia skupín alebo tímov v Office 365 v zozname adries
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811471"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrytie alebo zrušenie skrytia skupín alebo tímov v Office 365 v zozname adries

Ak chcete skryť alebo zrušiť skrytie skupiny alebo tímov v Office 365 v zoznamoch adries (GAL) klientov Exchange (Outlook, OWA), použite nasledujúci príkaz prostredia PowerShell EXO:

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Ak chcete skryť alebo zrušiť skrytie skupiny alebo tímov služieb Office365 v klientoch Exchange (Outlook, OWA), použite nasledujúci príkaz prostredia PowerShell EXO:

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Podrobné pokyny nájdete v téme [Skrytie skupín v Office 365 v rámci galícií a klientov Servera Exchange.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
