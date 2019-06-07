---
title: Nepodarilo sa odstrániť položky v SharePoint alebo OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757939"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="e459b-102">Nemožno odstrániť položky</span><span class="sxs-lookup"><span data-stu-id="e459b-102">Unable to delete items</span></span>

<span data-ttu-id="e459b-103">Problémy s odstránením položiek?</span><span class="sxs-lookup"><span data-stu-id="e459b-103">Having issues deleting items?</span></span>

- <span data-ttu-id="e459b-104">Vždy skontrolujte, či máte [príslušné povolenia](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) na odstrániť položku alebo mať [správca kolekcie lokality](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) pokus odstrániť položku.</span><span class="sxs-lookup"><span data-stu-id="e459b-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="e459b-105">Uistite sa, že nie je nastavenie [politiky uchovávania údajov](https://docs.microsoft.com/office365/securitycompliance/retention-policies) položky.</span><span class="sxs-lookup"><span data-stu-id="e459b-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="e459b-106">Uistite sa, či položka nie je [vzatý k sebe](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) iný používateľ.</span><span class="sxs-lookup"><span data-stu-id="e459b-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="e459b-107">Napokon, správcovia môžu pomocou [SharePoint vzorov a postupov](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ktorý obsahuje knižnicu PowerShell príkazy, ktoré vám umožnia vykonávať komplexné riadenie činnosti, ako napríklad sila odstránenie tvrdohlavý položiek.</span><span class="sxs-lookup"><span data-stu-id="e459b-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="e459b-108">Odstrániť PNP súbor</span><span class="sxs-lookup"><span data-stu-id="e459b-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="e459b-109">Odstrániť priečinok PNP</span><span class="sxs-lookup"><span data-stu-id="e459b-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="e459b-110">Odstrániť položku PNP</span><span class="sxs-lookup"><span data-stu-id="e459b-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="e459b-111">Odstrániť PNP</span><span class="sxs-lookup"><span data-stu-id="e459b-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="e459b-112">Odstrániť PNP pole (stĺpec)</span><span class="sxs-lookup"><span data-stu-id="e459b-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)