---
title: Riešenie problémov s odmietané správy programu Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758512"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="b4a05-102">Riešenie problémov s odmietané správy v službe SharePoint/OneDrive admin Center</span><span class="sxs-lookup"><span data-stu-id="b4a05-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="b4a05-103">Ak sa pri pokuse o prehľadávanie do centra spravovania služby SharePoint/OneDrive zobrazí hlásenie o odmietnutí prístupu, uistite sa, že ste [používateľovi priradili licenciu](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="b4a05-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="b4a05-104">Ak má používateľ licenciu, mali by ste sa tiež uistiť, že sú [priradené rolu správcu](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , ktorá má prístup do centra spravovania.</span><span class="sxs-lookup"><span data-stu-id="b4a05-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="b4a05-105">Tento problém sa môže vyskytnúť aj pri odstránení používateľa a znova vytvoriť s rovnakým hlavným menom používateľa (UPN).</span><span class="sxs-lookup"><span data-stu-id="b4a05-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="b4a05-106">Nový účet je vytvorený pomocou iného PUID (Passport unique ID) hodnotu.</span><span class="sxs-lookup"><span data-stu-id="b4a05-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="b4a05-107">Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo ich OneDrive, používateľ má nesprávne PUID.</span><span class="sxs-lookup"><span data-stu-id="b4a05-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="b4a05-108">Druhý scenár zahŕňa synchronizáciu adresárov s Active Directory organizačnú jednotku (OU).</span><span class="sxs-lookup"><span data-stu-id="b4a05-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="b4a05-109">Ak používatelia už prihlásení do služby SharePoint a potom sa premiestnia do iného OU a resynced s SharePoint, môžu sa vyskytnúť tento problém.</span><span class="sxs-lookup"><span data-stu-id="b4a05-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="b4a05-110">Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné UPN kroky v článku, [obnovenie používateľa v Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="b4a05-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="b4a05-111">Poznámka: Ak OneDrive alebo SharePoint admin Center nie je k dispozícii viacerým používateľom, ktorí predtým mali prístup, môže existovať dočasný problém služby.</span><span class="sxs-lookup"><span data-stu-id="b4a05-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="b4a05-112">[Skontrolujte stav služby tabuľa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b4a05-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


