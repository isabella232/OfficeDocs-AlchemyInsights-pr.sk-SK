---
title: Odstránenie súkromného kanála tímov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439915"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="2671f-102">Odstránenie súkromného kanála tímov</span><span class="sxs-lookup"><span data-stu-id="2671f-102">Delete a Teams private channel</span></span>

<span data-ttu-id="2671f-103">Spoločnosť Microsoft si je vedomá problému s odstránením súkromného kanála teams, ak máte pre príslušnú lokalitu SharePoint zapnutú politiku uchovávania údajov služby SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2671f-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="2671f-104">Spoločnosť Microsoft pracuje na opravu.</span><span class="sxs-lookup"><span data-stu-id="2671f-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="2671f-105">Medzitým môžete použiť nasledujúce riešenia na odstránenie súkromného kanála.</span><span class="sxs-lookup"><span data-stu-id="2671f-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="2671f-106">**Vylúčiť tímovú kolekciu alebo kolekciu lokalít z politiky uchovávania údajov lokality Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="2671f-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="2671f-107">Prejdite na portál na správu služieb Office 365 a na **ľavej navigačnej table** vyberte položku Zobraziť všetko.</span><span class="sxs-lookup"><span data-stu-id="2671f-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="2671f-108">V **časti Centrá spravovania prejdite**na **položku & zásady**  >  **ochrany údajov**o dodržiavaní  >  **súladu**.</span><span class="sxs-lookup"><span data-stu-id="2671f-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="2671f-109">Identifikujte všetky politiky, ktoré sa vzťahujú na lokality Sharepoint, a upravte politiku tak, aby lokalita Sharepoint pre tím obsahujúci súkromný kanál nebola zahrnutá do politiky uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="2671f-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="2671f-110">Uložte politiku.</span><span class="sxs-lookup"><span data-stu-id="2671f-110">Save the policy.</span></span>
    <span data-ttu-id="2671f-111">Môže trvať až 24 hodín, kým sa nastavenia politiky prejavia.</span><span class="sxs-lookup"><span data-stu-id="2671f-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="2671f-112">Po vylúčení lokality môžete súkromný kanál odstrániť.</span><span class="sxs-lookup"><span data-stu-id="2671f-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="2671f-113">Súkromný ***kanál*** môžete odstrániť pomocou služby Microsoft Teams v zariadení s Androidom.</span><span class="sxs-lookup"><span data-stu-id="2671f-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="2671f-114">Súvisiace informácie o SharePointe nájdete v [téme Nie je možné odstrániť položky v SharePointe Online alebo OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="2671f-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>