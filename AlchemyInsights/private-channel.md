---
title: Súkromný kanál
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005453"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="8a349-102">Súkromné kanály v Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="8a349-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="8a349-103">Súkromné kanály sú novou funkciou v Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="8a349-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="8a349-104">Upozorňujeme, že súkromné kanály nemožno konvertovať zo štandardných kanálov ani naopak.</span><span class="sxs-lookup"><span data-stu-id="8a349-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="8a349-105">Podrobnosti o súkromných kanáloch, ako sú napríklad informácie o [vytváraní privátneho kanála a o členstve](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) a [súkromných kanáloch lokality SharePoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), nájdete [v téme súkromné kanály v Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="8a349-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="8a349-106">**Poznámka:** Keďže Konfigurácia uchovávania súkromných správ kanála ešte nie je podporovaná, nájomníci s povolenými politikami uchovávania údajov nebudú mať predvolene povolené súkromné kanály.</span><span class="sxs-lookup"><span data-stu-id="8a349-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="8a349-107">Súkromné kanály môžu byť povolené v tíme admin Center.</span><span class="sxs-lookup"><span data-stu-id="8a349-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="8a349-108">Všimnite si tiež, že zatiaľ čo uchovávanie súkromných kanálov správ nie je podporovaný, je podporovaný uchovávanie súborov zdieľaných v súkromných kanáloch.</span><span class="sxs-lookup"><span data-stu-id="8a349-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="8a349-109">**Potrebujete nového vlastníka tímu?**</span><span class="sxs-lookup"><span data-stu-id="8a349-109">**Need a new team owner?**</span></span>

<span data-ttu-id="8a349-110">Ak váš súkromný kanál vlastník opustí, môžete pridať nového vlastníka tímu cez tímy PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8a349-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="8a349-111">Choď [sem](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) nainštalovať tímy PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8a349-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="8a349-112">Tu je rutina cmdlet budete potrebovať:</span><span class="sxs-lookup"><span data-stu-id="8a349-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="8a349-113">Ďalšie informácie o tímových PowerShell, pozri [tímy PowerShell prehľad](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="8a349-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
