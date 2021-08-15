---
title: Zapnutie technológie NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023537"
---
# <a name="turn-on-ndi-technology"></a>Zapnutie technológie NDI

Technológia NDI vyžaduje, aby používateľ zapol dva kroky:

1. Správca nájomníkov musí povoliť vlastnosť AllowNDIStreaming v časti CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Po zaplnení tejto zmeny musí koncový používateľ zapnúť technológiu NDI® pre svojho konkrétneho klienta **z Nastavenia > povolení.**

Ďalšie informácie nájdete v téme [Používanie technológie NDI v Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
