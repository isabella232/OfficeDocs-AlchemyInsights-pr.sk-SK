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
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935138"
---
# <a name="turn-on-ndi-technology"></a>Zapnutie technológie NDI

Technológia NDI vyžaduje, aby sa pre používateľa zapli dva kroky:

1. Správca nájomníkov musí povoliť vlastnosť AllowNDIStreaming v CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Po vyplnení tejto zmeny musí koncový používateľ zapnúť technológiu NDI® pre konkrétneho klienta v **nastaveniach > povolení**.

Ďalšie informácie nájdete v téme [Používanie technológie NDI v aplikácii Microsoft teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
