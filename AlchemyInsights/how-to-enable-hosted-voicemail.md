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
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="e2833-102">Povolenie hosťovanej hlasovej schránky</span><span class="sxs-lookup"><span data-stu-id="e2833-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="e2833-103">Ak chcete povoliť hlasovú schránku, **HostedVoicemail** musí byť nastavená na možnosť $true.</span><span class="sxs-lookup"><span data-stu-id="e2833-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="e2833-104">Vlastnosť **HostedVoicemail** používateľa pomocou vzdialeného prostredia POWERSHELL (RPR).</span><span class="sxs-lookup"><span data-stu-id="e2833-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="e2833-105">Ďalšie informácie o pripojení k RPR nájdete v téme [Microsoft teams PowerShell – prehľad](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pre ďalšie informácie o pripájaní k RPR.</span><span class="sxs-lookup"><span data-stu-id="e2833-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="e2833-106">Správca tímov by sa mal prihlásiť do vzdialeného prostredia PowerShell pre teams.</span><span class="sxs-lookup"><span data-stu-id="e2833-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="e2833-107">Príkaz v prostredí PowerShell môže správca tímov spustiť **set-csuser user@contoso.com-HostedVoiceMail $True** , kde je identifikátor SIP URI príslušného používateľa.</span><span class="sxs-lookup"><span data-stu-id="e2833-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="e2833-108">Zmeny politiky môžu trvať až 24 hodín, kým sa replikujú.</span><span class="sxs-lookup"><span data-stu-id="e2833-108">Changes to policies can take up to 24 hours to replicate.</span></span>