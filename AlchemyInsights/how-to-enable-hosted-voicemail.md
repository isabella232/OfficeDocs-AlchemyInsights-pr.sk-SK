---
title: Zapnutie hosťovanej hlasovej schránky
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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055569"
---
# <a name="how-to-enable-hosted-voicemail"></a>Zapnutie hosťovanej hlasovej schránky

Ak chcete povoliť hlasovú schránku, musí byť služba **HostedVoicemail** nastavená na možnosť $true.

Vlastnosť **HostedVoicemail** používateľa pomocou prostredia Remote PowerShell (RPS).

Ďalšie informácie o pripojení k RPS nájdete v téme [Prehľad prostredia PowerShell Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) informácie o pripojení k RPS.

1. Správca Teams by mal byť prihlásený do prostredia Remote PowerShell pre Teams.
1. V príkazovom riadku prostredia PowerShell môže správca Teams spustiť rutinu **set-csuser user@contoso.com -HostedVoiceMail $true,** kde je uri s sip uri v otázke.

> [!NOTE]
> Replikovať zmeny politík môžu trvať až 24 hodín.