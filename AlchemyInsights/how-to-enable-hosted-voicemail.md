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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318663"
---
# <a name="how-to-enable-hosted-voicemail"></a>Zapnutie hosťovanej hlasovej schránky

Ak chcete povoliť hlasovú schránku, musí byť služba **HostedVoicemail** nastavená na možnosť $true.

Vlastnosť **HostedVoicemail** používateľa pomocou prostredia Remote PowerShell (RPS).

Ďalšie informácie o pripojení k RPS nájdete v téme Prehľad [prostredia PowerShell Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) informácie o pripojení k RPS.

1. Správca Teams by mal byť prihlásený do prostredia Remote PowerShell pre Teams.
1. V príkazovom riadku prostredia PowerShell môže správca Teams spustiť rutinu **set-csuser user@contoso.com -HostedVoiceMail $true,** kde je uri s sip uri v otázke.

**Poznámka:** Replikovať zmeny politík môžu trvať až 24 hodín.