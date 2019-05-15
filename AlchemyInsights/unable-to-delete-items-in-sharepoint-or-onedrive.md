---
title: Nepodarilo sa odstrániť položky v SharePoint alebo OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057772"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="4f232-102">Nemožno odstrániť položky</span><span class="sxs-lookup"><span data-stu-id="4f232-102">Unable to delete items</span></span>

<span data-ttu-id="4f232-103">Problémy s odstránením položiek?</span><span class="sxs-lookup"><span data-stu-id="4f232-103">Having issues deleting items?</span></span>

- <span data-ttu-id="4f232-104">Vždy skontrolujte, či máte [príslušné povolenia](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) na odstrániť položku alebo mať [správca kolekcie lokality](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) pokus odstrániť položku.</span><span class="sxs-lookup"><span data-stu-id="4f232-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="4f232-105">Uistite sa, že nie je nastavenie [politiky uchovávania údajov](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) položky.</span><span class="sxs-lookup"><span data-stu-id="4f232-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="4f232-106">Uistite sa, či položka nie je [vzatý k sebe](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) iný používateľ.</span><span class="sxs-lookup"><span data-stu-id="4f232-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="4f232-107">Napokon, správcovia môžu pomocou [SharePoint vzorov a postupov](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ktorý obsahuje knižnicu PowerShell príkazy, ktoré vám umožnia vykonávať komplexné riadenie činnosti, ako napríklad sila odstránenie tvrdohlavý položiek.</span><span class="sxs-lookup"><span data-stu-id="4f232-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="4f232-108">Odstrániť PNP súbor</span><span class="sxs-lookup"><span data-stu-id="4f232-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="4f232-109">Odstrániť priečinok PNP</span><span class="sxs-lookup"><span data-stu-id="4f232-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="4f232-110">Odstrániť položku PNP</span><span class="sxs-lookup"><span data-stu-id="4f232-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="4f232-111">Odstrániť PNP</span><span class="sxs-lookup"><span data-stu-id="4f232-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="4f232-112">Odstrániť PNP pole (stĺpec)</span><span class="sxs-lookup"><span data-stu-id="4f232-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)