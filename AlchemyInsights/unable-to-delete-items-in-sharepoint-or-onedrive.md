---
title: Nie je možné odstrániť položky v službe SharePoint alebo OneDrive
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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571286"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="f9704-102">Položky sa nedajú odstrániť</span><span class="sxs-lookup"><span data-stu-id="f9704-102">Unable to delete items</span></span>

<span data-ttu-id="f9704-103">Politiky uchovávania údajov môžu spôsobiť to, musíte buď vypnúť alebo vylúčiť príslušné zadržanie, ktoré spôsobuje tento problém.</span><span class="sxs-lookup"><span data-stu-id="f9704-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="f9704-104">Po odstránení politiky uchovávania alebo zadržania môže zmena trvať až 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="f9704-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="f9704-105">Uistite sa, že na položku nie je nastavenie [politiky uchovávania údajov](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="f9704-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="f9704-106">Lokalita mohla prekročiť limit ukladacieho priestoru, zvýšiť [kvótu lokality](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) a odstrániť položku.</span><span class="sxs-lookup"><span data-stu-id="f9704-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="f9704-107">Uistite sa, že položka nie je [vzatý](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) k sebe inému používateľovi.</span><span class="sxs-lookup"><span data-stu-id="f9704-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="f9704-108">Nakoniec, správcovia môžu používať [SharePoint vzory a postupy](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ktorý obsahuje knižnicu príkazov PowerShell, ktoré umožňujú vykonávať komplexné riadenie akcie, ako je sila odstránenie tvrdohlavý položky.</span><span class="sxs-lookup"><span data-stu-id="f9704-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="f9704-109">Odstrániť súbor PNP</span><span class="sxs-lookup"><span data-stu-id="f9704-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="f9704-110">Odstrániť priečinok PNP</span><span class="sxs-lookup"><span data-stu-id="f9704-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="f9704-111">Odstrániť položku zoznamu PNP</span><span class="sxs-lookup"><span data-stu-id="f9704-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="f9704-112">Odstrániť zoznam PNP</span><span class="sxs-lookup"><span data-stu-id="f9704-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="f9704-113">Odstrániť pole PNP (stĺpec)</span><span class="sxs-lookup"><span data-stu-id="f9704-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)