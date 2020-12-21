---
title: Správa skupín aplikácií pomocou platformy Azure Portal pre Windows Virtual Desktop
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
- "9003956"
- "7013"
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722056"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a><span data-ttu-id="dd707-102">Správa skupín aplikácií pomocou platformy Azure Portal pre Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="dd707-102">Manage app groups by using the Azure portal for Windows Virtual Desktop</span></span>

<span data-ttu-id="dd707-103">Predvolená skupina aplikácií vytvorená pre nový Windows Virtual Desktop Host pool tiež publikuje celú pracovnú plochu.</span><span class="sxs-lookup"><span data-stu-id="dd707-103">The default app group created for a new Windows Virtual Desktop host pool also publishes the full desktop.</span></span> <span data-ttu-id="dd707-104">Pomocou portálu Azure môžete okrem toho vytvoriť jednu alebo viacero skupín aplikácií RemoteApp pre hostiteľský fond.</span><span class="sxs-lookup"><span data-stu-id="dd707-104">In addition, using the Azure portal lets you create one or more RemoteApp app groups for the host pool.</span></span>

<span data-ttu-id="dd707-105">Proces nasadenia bude nasledovný:</span><span class="sxs-lookup"><span data-stu-id="dd707-105">The deployment process will do the following:</span></span>

1. <span data-ttu-id="dd707-106">Vytvorte skupinu aplikácií RemoteApp.</span><span class="sxs-lookup"><span data-stu-id="dd707-106">Create the RemoteApp app group.</span></span>
2. <span data-ttu-id="dd707-107">Pridajte vybraté aplikácie do skupiny aplikácií.</span><span class="sxs-lookup"><span data-stu-id="dd707-107">Add your selected apps to the app group.</span></span>
3. <span data-ttu-id="dd707-108">Publikujte jednotlivých používateľov alebo skupiny používateľov do skupiny aplikácií.</span><span class="sxs-lookup"><span data-stu-id="dd707-108">Publish individual users or user groups to the app group.</span></span>
4. <span data-ttu-id="dd707-109">Zaregistrujte skupinu aplikácií, ak sa tak rozhodnete.</span><span class="sxs-lookup"><span data-stu-id="dd707-109">Register the app group, if you choose to do so.</span></span>
5. <span data-ttu-id="dd707-110">Vytvorte prepojenie na šablónu nástroja Azure Resource Manager v závislosti od konfigurácie, ktorú si môžete stiahnuť a uložiť.</span><span class="sxs-lookup"><span data-stu-id="dd707-110">Create a link to an Azure Resource Manager template according to your configuration, which you can download and save.</span></span>

<span data-ttu-id="dd707-111">Ak chcete vytvoriť skupinu RemoteApp pre virtuálnu pracovnú plochu Windowsu, postupujte podľa pokynov v téme [Správa skupín aplikácií pomocou portálu Azure](https://go.microsoft.com/fwlink/?linkid=2129550).</span><span class="sxs-lookup"><span data-stu-id="dd707-111">To create a RemoteApp group for Windows Virtual Desktop, follow the instructions in [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span></span>
