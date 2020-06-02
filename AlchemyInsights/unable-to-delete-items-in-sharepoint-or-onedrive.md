---
title: Nie je možné odstrániť položky v SharePointe alebo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511991"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="75134-102">Nie je možné odstrániť položky</span><span class="sxs-lookup"><span data-stu-id="75134-102">Unable to delete items</span></span>

<span data-ttu-id="75134-103">Politiky uchovávania údajov môže spôsobiť, musíte vypnúť alebo vylúčiť príslušné zadržanie, ktoré spôsobuje tento problém.</span><span class="sxs-lookup"><span data-stu-id="75134-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="75134-104">Po odstránení politiky uchovávania údajov alebo zadržaní môže trvať až 24 hodín, kým sa zmena prejaví.</span><span class="sxs-lookup"><span data-stu-id="75134-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="75134-105">Skontrolujte, či v položke nie je nastavenie [politiky uchovávania údajov.](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)</span><span class="sxs-lookup"><span data-stu-id="75134-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="75134-106">Lokalita mohla prekročiť limit ukladacieho priestoru, zvýšiť [kvótu lokality](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) a odstrániť položku.</span><span class="sxs-lookup"><span data-stu-id="75134-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="75134-107">Skontrolujte, či položka nie je [vzatá k sebe](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) inému používateľovi.</span><span class="sxs-lookup"><span data-stu-id="75134-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="75134-108">Nakoniec správcovia môžu používať [SharePoint vzory a postupy](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ktorý obsahuje knižnicu príkazov prostredia PowerShell, ktoré umožňujú vykonávať zložité akcie správy, ako je napríklad vynútenie odstránenia tvrdohlavých položiek.</span><span class="sxs-lookup"><span data-stu-id="75134-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="75134-109">Odstrániť pnp súbor</span><span class="sxs-lookup"><span data-stu-id="75134-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="75134-110">Odstrániť pnp priečinok</span><span class="sxs-lookup"><span data-stu-id="75134-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="75134-111">Odstrániť položku zoznamu PNP</span><span class="sxs-lookup"><span data-stu-id="75134-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="75134-112">Odstrániť pnp zoznam</span><span class="sxs-lookup"><span data-stu-id="75134-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="75134-113">Odstrániť pole PNP (stĺpec)</span><span class="sxs-lookup"><span data-stu-id="75134-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)