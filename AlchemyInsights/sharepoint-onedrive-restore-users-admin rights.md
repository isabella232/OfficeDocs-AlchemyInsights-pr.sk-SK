---
title: Riešenie problémov s prístupom odmietnutých správ na lokality služby OneDrive for Business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670631"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="34a8f-102">Riešenie problémov s prístupom odmietnutých správ na lokality služby OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="34a8f-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="34a8f-103">Tento problém sa vyskytuje najčastejšie pri odstránení používateľa a opätovnom vytvorení s rovnakým hlavným menom používateľa (UPN).</span><span class="sxs-lookup"><span data-stu-id="34a8f-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="34a8f-104">Nové konto sa vytvorí s použitím inej hodnoty PUID (jedinečného ID konta Passport).</span><span class="sxs-lookup"><span data-stu-id="34a8f-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="34a8f-105">Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo k ich OneDrivu, má používateľ nesprávny PUID.</span><span class="sxs-lookup"><span data-stu-id="34a8f-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="34a8f-106">Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="34a8f-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="34a8f-107">Ak sa používatelia už prihlásili do SharePointu a potom sa prenesú do inej OU a opätovne sa synchronizujú so SharePointom, tento problém sa môže vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="34a8f-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="34a8f-108">Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné meno používateľa podľa krokov v článku [obnovenie používateľa v programe Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="34a8f-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="34a8f-109">Ak nie je možné obnoviť pôvodného používateľa, mali by ste odstrániť starého používateľa z lokality OneDrive pomocou týchto krokov, [odstrániť používateľa zo zoznamu informácie o používateľoch]().</span><span class="sxs-lookup"><span data-stu-id="34a8f-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="34a8f-110">Po dokončení tohto postupu môžete overiť, či má používateľ práva správcu na lokalitu OneDrive, a to pomocou krokov na [Pridanie správcu pre OneDrive používateľa](https://docs.microsoft.com/sharepoint/manage-user-profiles) .</span><span class="sxs-lookup"><span data-stu-id="34a8f-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="34a8f-111">Ďalšie informácie o úrovniach povolení nájdete v článku [Vysvetlenie úrovní povolení v SharePointe](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="34a8f-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
