---
title: Skrytie verejných priečinkov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315439"
---
# <a name="hide-public-folders"></a><span data-ttu-id="b775d-102">Skrytie verejných priečinkov</span><span class="sxs-lookup"><span data-stu-id="b775d-102">Hide public folders</span></span>

<span data-ttu-id="b775d-103">**Skrytie celého verejného stromu priečinkov**:</span><span class="sxs-lookup"><span data-stu-id="b775d-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="b775d-104">Pomocou krokov v [tomto](https://aka.ms/ControlPF) článku skryjete celý verejný strom priečinkov od selektívnych alebo všetkých používateľov.</span><span class="sxs-lookup"><span data-stu-id="b775d-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="b775d-105">**Skrytie konkrétneho verejného priečinka**:</span><span class="sxs-lookup"><span data-stu-id="b775d-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="b775d-106">Pridanie povolení pre používateľov, ktorí potrebujú prístup k verejnému priečinku</span><span class="sxs-lookup"><span data-stu-id="b775d-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="b775d-107">Odstránenie **predvoleného** používateľa zo zoznamu **povolení** :</span><span class="sxs-lookup"><span data-stu-id="b775d-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
