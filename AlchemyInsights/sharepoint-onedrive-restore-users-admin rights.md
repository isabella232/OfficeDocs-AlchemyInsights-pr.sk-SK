---
title: Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051620"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="456f0-102">Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality</span><span class="sxs-lookup"><span data-stu-id="456f0-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="456f0-103">Tento problém sa vyskytuje najčastejšie pri odstránení používateľa a znova vytvoriť s rovnakým hlavným menom používateľa (UPN).</span><span class="sxs-lookup"><span data-stu-id="456f0-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="456f0-104">Nový účet je vytvorený pomocou iného PUID (Passport unique ID) hodnotu.</span><span class="sxs-lookup"><span data-stu-id="456f0-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="456f0-105">Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo ich OneDrive, používateľ má nesprávne PUID.</span><span class="sxs-lookup"><span data-stu-id="456f0-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="456f0-106">Druhý scenár zahŕňa synchronizáciu adresárov s Active Directory organizačnú jednotku (OU).</span><span class="sxs-lookup"><span data-stu-id="456f0-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="456f0-107">Ak používatelia už prihlásení do služby SharePoint a potom sa premiestnia do iného OU a resynced s SharePoint, môžu sa vyskytnúť tento problém.</span><span class="sxs-lookup"><span data-stu-id="456f0-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="456f0-108">Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné UPN kroky v článku, [obnovenie používateľa v balíku Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="456f0-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="456f0-109">Ak nemôžete obnoviť pôvodného používateľa, mali by ste odstrániť starého používateľa z OneDrive stránky pomocou týchto krokov, [odstrániť používateľa zo zoznamu informácie o používateľovi]().</span><span class="sxs-lookup"><span data-stu-id="456f0-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="456f0-110">Po dokončení tohto postupu môžete overiť, že používateľ má administrátorské práva na lokalitu OneDrive podľa krokov na [Pridanie admin pre používateľa OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="456f0-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="456f0-111">Ďalšie informácie o úrovniach povolení nájdete [v článku Vysvetlenie úrovní povolení v službe SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="456f0-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
