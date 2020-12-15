---
title: Povolenie hosťovanej hlasovej schránky
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679166"
---
# <a name="how-to-enable-hosted-voicemail"></a>Povolenie hosťovanej hlasovej schránky

Ak chcete povoliť hlasovú schránku, **HostedVoicemail** musí byť nastavená na možnosť $true.

Vlastnosť **HostedVoicemail** používateľa pomocou vzdialeného prostredia POWERSHELL (RPR).

Ďalšie informácie o pripojení k RPR nájdete v téme [Microsoft teams PowerShell – prehľad](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pre ďalšie informácie o pripájaní k RPR.

1. Správca tímov by sa mal prihlásiť do vzdialeného prostredia PowerShell pre teams.
1. Príkaz v prostredí PowerShell môže správca tímov spustiť **set-csuser user@contoso.com-HostedVoiceMail $True** , kde je identifikátor SIP URI príslušného používateľa.

> [!NOTE]
> Zmeny politiky môžu trvať až 24 hodín, kým sa replikujú.