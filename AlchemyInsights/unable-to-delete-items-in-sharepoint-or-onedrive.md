---
title: Nie je možné odstrániť položky v SharePointe alebo vo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806126"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="c4195-102">Nie je možné odstrániť položky</span><span class="sxs-lookup"><span data-stu-id="c4195-102">Unable to delete items</span></span>

<span data-ttu-id="c4195-103">Politiky uchovávania údajov môžu spôsobiť, že je potrebné vypnúť alebo vylúčiť príslušné zadržanie, ktoré spôsobuje tento problém.</span><span class="sxs-lookup"><span data-stu-id="c4195-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="c4195-104">Po odstránení politiky alebo zadržania uchovávania údajov môže zmena nadobudnúť až 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="c4195-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="c4195-105">Skontrolujte, či sa v položke nenachádza nastavenie [politiky uchovávania údajov](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="c4195-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="c4195-106">Lokalita mohla prekročila limit ukladacieho priestoru, zvýšiť [kvótu lokality](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) a odstrániť ju.</span><span class="sxs-lookup"><span data-stu-id="c4195-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="c4195-107">Uistite sa, že položka nie je [vzatá z projektu](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) inému používateľovi.</span><span class="sxs-lookup"><span data-stu-id="c4195-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="c4195-108">Správcovia môžu nakoniec použiť [vzorce a postupy SharePointu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ktoré obsahujú knižnicu príkazov prostredia PowerShell, ktoré vám umožňujú vykonávať zložité akcie spravovania, ako je napríklad vynútiť odstraňovanie nepoddajných položiek.</span><span class="sxs-lookup"><span data-stu-id="c4195-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="c4195-109">Odstránenie súboru PNP</span><span class="sxs-lookup"><span data-stu-id="c4195-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="c4195-110">Odstránenie priečinka PNP</span><span class="sxs-lookup"><span data-stu-id="c4195-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="c4195-111">Odstránenie položky zoznamu PNP</span><span class="sxs-lookup"><span data-stu-id="c4195-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="c4195-112">Odstrániť zoznam PNP</span><span class="sxs-lookup"><span data-stu-id="c4195-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="c4195-113">Odstrániť pole PNP (stĺpec)</span><span class="sxs-lookup"><span data-stu-id="c4195-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)