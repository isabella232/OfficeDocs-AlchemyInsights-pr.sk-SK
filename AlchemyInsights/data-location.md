---
title: Umiestnenie údajov
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627861"
---
# <a name="data-location"></a><span data-ttu-id="7d278-102">Umiestnenie údajov</span><span class="sxs-lookup"><span data-stu-id="7d278-102">Data location</span></span>

<span data-ttu-id="7d278-103">Umiestnenie nájomníka balíka Office 365 môžete zobraziť v centre spravovania alebo pripojením na Exchange Online cez PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7d278-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="7d278-104">**Admin Center:**</span><span class="sxs-lookup"><span data-stu-id="7d278-104">**Admin center:**</span></span>
1. <span data-ttu-id="7d278-105">Prihláste sa do [centra spravovania](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="7d278-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="7d278-106">Vyberte položku **Nastavenie** > **profilu organizácie**.</span><span class="sxs-lookup"><span data-stu-id="7d278-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="7d278-107">V časti **Umiestnenie údajov**vyberte položku **Zobraziť podrobnosti**.</span><span class="sxs-lookup"><span data-stu-id="7d278-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="7d278-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="7d278-108">**PowerShell:**</span></span>
1. <span data-ttu-id="7d278-109">Pripojenie k službe Exchange Online pomocou prostredia Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7d278-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="7d278-110">Spustiť rutiny cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) Zobraziť zoznam vlastností nájomcu.</span><span class="sxs-lookup"><span data-stu-id="7d278-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="7d278-111">Pozrite sa na vlastnosť OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="7d278-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="7d278-112">Ak máte umiestnenie údajov pre EXO a SPO, môžete určiť umiestnenie údajov pre iné služby, ktoré môžete použiť z [miesta, kde sa vaše údaje nachádzajú](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="7d278-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>