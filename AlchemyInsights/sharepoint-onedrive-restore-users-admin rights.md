---
title: Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223439"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="dcc12-102">Riešenie problémov prístup odmietnutý správy OneDrive pre podnikové lokality</span><span class="sxs-lookup"><span data-stu-id="dcc12-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="dcc12-103">Tento problém sa vyskytuje najčastejšie keď používateľ odstráni a znova vytvorí s rovnaké hlavné meno používateľa (UPN).</span><span class="sxs-lookup"><span data-stu-id="dcc12-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="dcc12-104">Nové konto je vytvorený pomocou rôznych PUID služby (Passport jedinečný identifikátor) hodnotu.</span><span class="sxs-lookup"><span data-stu-id="dcc12-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="dcc12-105">Keď sa používateľ pokúsi prístup kolekcie lokalít alebo ich OneDrive, používateľ má nesprávny PUID služby.</span><span class="sxs-lookup"><span data-stu-id="dcc12-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="dcc12-106">Druhý scenár zahŕňa adresár synchronizácia so Active Directory organizačnú jednotku (OU).</span><span class="sxs-lookup"><span data-stu-id="dcc12-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="dcc12-107">Ak používatelia už prihlásený do služby SharePoint, a potom sa presunie na rôznych OU a resynced so službou SharePoint, tento problém sa môže vyskytnúť.</span><span class="sxs-lookup"><span data-stu-id="dcc12-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="dcc12-108">Na vyriešenie tohto problému by ste mali obnoviť pôvodný UPN s kroky v tomto článku,[obnovení používateľa v balíku Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="dcc12-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="dcc12-109">Po sa to deje, môžete si overiť má používateľ admin práva na OneDrive stránky pomocou nasledujúcich krokov na [Pridanie admin's používateľa OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="dcc12-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="dcc12-110">Ďalšie informácie o úrovniach povolení nájdete v článku [pochopenie úrovne povolení v službe SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="dcc12-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
