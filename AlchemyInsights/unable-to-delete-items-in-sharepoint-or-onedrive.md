---
title: Nie je možné odstrániť položky v službe SharePoint alebo OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748591"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="65549-102">Položky sa nedajú odstrániť</span><span class="sxs-lookup"><span data-stu-id="65549-102">Unable to delete items</span></span>

<span data-ttu-id="65549-103">Máte problémy s odstránením položiek služby SharePoint?</span><span class="sxs-lookup"><span data-stu-id="65549-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="65549-104">Vždy sa uistite, že máte [príslušné povolenia](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) na odstránenie položky alebo sa pokúsi odstrániť položku [správca kolekcie lokalít](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) .</span><span class="sxs-lookup"><span data-stu-id="65549-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="65549-105">Uistite sa, že na položku nie je nastavenie [politiky uchovávania údajov](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="65549-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="65549-106">Uistite sa, že položka nie je [vzatý](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) k sebe inému používateľovi.</span><span class="sxs-lookup"><span data-stu-id="65549-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="65549-107">Nakoniec, správcovia môžu používať [SharePoint vzory a postupy](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ktorý obsahuje knižnicu príkazov PowerShell, ktoré umožňujú vykonávať komplexné riadenie akcie, ako je sila odstránenie tvrdohlavý položky.</span><span class="sxs-lookup"><span data-stu-id="65549-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="65549-108">Odstrániť súbor PNP</span><span class="sxs-lookup"><span data-stu-id="65549-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="65549-109">Odstrániť priečinok PNP</span><span class="sxs-lookup"><span data-stu-id="65549-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="65549-110">Odstrániť položku zoznamu PNP</span><span class="sxs-lookup"><span data-stu-id="65549-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="65549-111">Odstrániť zoznam PNP</span><span class="sxs-lookup"><span data-stu-id="65549-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="65549-112">Odstrániť pole PNP (stĺpec)</span><span class="sxs-lookup"><span data-stu-id="65549-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)