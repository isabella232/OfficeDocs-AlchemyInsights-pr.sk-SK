---
title: Používanie Giphy v konverzáciách v aplikácii teams
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
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982578"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="adb59-102">Používanie Giphy v konverzáciách v aplikácii teams</span><span class="sxs-lookup"><span data-stu-id="adb59-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="adb59-103">Giphy Access v aplikácii teams chat je predvolene zapnutý.</span><span class="sxs-lookup"><span data-stu-id="adb59-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="adb59-104">Ako správca môžete ovládať, či sú Giphy k dispozícii pre používateľov [nastavením politiky odosielania správ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) a zabezpečte, aby bolo **zapnuté** **Používanie giphy v konverzáciách** .</span><span class="sxs-lookup"><span data-stu-id="adb59-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="adb59-105">Ak GIF nefungujú podľa očakávaní v konverzáciách v aplikácii Teams, overte:</span><span class="sxs-lookup"><span data-stu-id="adb59-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="adb59-106">[Politika odosielania správ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) musí povoľovať giphy.</span><span class="sxs-lookup"><span data-stu-id="adb59-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="adb59-107">Overenie pomocou rutiny typu cmdlet prostredia PowerShell:</span><span class="sxs-lookup"><span data-stu-id="adb59-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="adb59-108">Overte, či môžete [Spravovať tímy s prostredím PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="adb59-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="adb59-109">Spustite príkaz prostredia PowerShell [Get-CsTeamsMessagingPolicy-identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) a overte, či je **AllowGiphy** nastavený na **hodnotu True**.</span><span class="sxs-lookup"><span data-stu-id="adb59-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="adb59-110">Ak je **AllowGiphy** nastavený na **hodnotu False** , spustite nasledujúci príkaz v prostredí PowerShell – [CsTeamsMessagingPolicy-identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="adb59-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="adb59-111">[Voliteľné pripojené](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) funkcie je potrebné povoliť na umožnenie prístupu k URL adrese Giphy.</span><span class="sxs-lookup"><span data-stu-id="adb59-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="adb59-112">Ak máte v nájomníkovi nakonfigurované viaceré politiky na výmenu správ, môžete určiť identitu politiky priradenej k ovplyvnenému používateľovi s príkazom prostredia PowerShell [Get-CsOnlineUser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Vyberte položku TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="adb59-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
