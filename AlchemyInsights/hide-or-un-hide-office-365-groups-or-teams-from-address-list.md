---
title: Skrytie alebo zrušenie Office 365 skupín alebo tímov v zozname adries
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088411"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrytie alebo zrušenie Office 365 skupín alebo tímov v zozname adries

Pomocou nasledujúceho príkazu prostredia PowerShell EXO môžete skryť alebo zrušiť Office 365 skupiny alebo tímy v zoznamoch adries (GAL) Exchange klientoch (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Ak chcete skryť alebo zrušiť skrytie skupiny alebo tímov v Office365 v klientoch služieb Exchange (Outlook, OWA), použite nasledujúci príkaz prostredia PowerShell:

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Podrobné pokyny nájdete v téme [skrytie Office 365 skupín v galícii a Exchange klientoch.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
