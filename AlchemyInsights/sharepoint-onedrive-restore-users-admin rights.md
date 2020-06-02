---
title: Riešenie problémov s prístupom odmietnutýsprávy onedrive business lokality
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511199"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="d9f9c-102">Riešenie problémov s prístupom odmietnutýsprávy onedrive business lokality</span><span class="sxs-lookup"><span data-stu-id="d9f9c-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="d9f9c-103">Tento problém sa najčastejšie vyskytuje, keď sa používateľ odstráni a znova vytvorí s rovnakým hlavným menom používateľa (UPN).</span><span class="sxs-lookup"><span data-stu-id="d9f9c-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="d9f9c-104">Nové konto sa vytvorí pomocou inej hodnoty PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="d9f9c-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="d9f9c-105">Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo onedrive, používateľ má nesprávne PUID.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="d9f9c-106">Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="d9f9c-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="d9f9c-107">Ak sa používatelia už prihlásili do služby SharePoint a potom sa premiestnia do inej ou a znova synchronizujú so službou SharePoint, môžu sa vyskytnúť tento problém.</span><span class="sxs-lookup"><span data-stu-id="d9f9c-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="d9f9c-108">Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné UPN s krokmi v článku [Obnoviť používateľa v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="d9f9c-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="d9f9c-109">Ak nemôžete obnoviť pôvodného používateľa, mali by ste odstrániť starého používateľa z lokality OneDrive pomocou týchto krokov, [Odstráňte používateľa zo zoznamu informácií o používateľovi]().</span><span class="sxs-lookup"><span data-stu-id="d9f9c-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="d9f9c-110">Po vykonaní tohto postupu môžete overiť, že používateľ má práva správcu na lokalitu OneDrive podľa krokov na [pridanie správcu pre používateľa OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="d9f9c-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="d9f9c-111">Ďalšie informácie o úrovniach povolení nájdete v článku [Informácie o úrovniach povolení v SharePointe](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="d9f9c-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
