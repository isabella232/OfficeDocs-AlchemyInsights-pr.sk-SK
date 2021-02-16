---
title: Povolenie zariadenia
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256983"
---
# <a name="enable-device"></a>Povolenie zariadenia

**Povolenie zariadenia pomocou príkazu prostredia PowerShell**

Spustite nasledujúce príkazy:

- Ak chcete získať objekt zariadenia: `Get-MsolDevice -Name <Name>`
- Povolenie zariadenia: `Enable-MsolDevice -DeviceId <DeviceId>`

Ďalšie informácie o konfigurácii hybridného spojenia v spravovaných doménach nájdete v téme [Konfigurácia hybridného spojenia](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
