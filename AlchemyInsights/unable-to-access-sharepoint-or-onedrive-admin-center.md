---
title: Nie je možné získať prístup do Centra spravovania služby SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824450"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="b8ce3-102">Nie je možné získať prístup do Centra spravovania služby SharePoint alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="b8ce3-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="b8ce3-103">Ak je lokalita Centra spravovania služby SharePoint alebo OneDrive nedostupná alebo nedostupná, môže ísť o dočasný problém so službou, pri ktorom sa používateľom pri prístupe k lokalitám SharePoint alebo obsahu vo OneDrive vyskytujú občasné oneskorenia alebo chyby navigácie.</span><span class="sxs-lookup"><span data-stu-id="b8ce3-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="b8ce3-104">Na [tabuli Stav služby](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) zistite, či to bude mať vplyv na vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="b8ce3-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="b8ce3-105">Globálni správcovia a správcovia služby SharePoint musia mať priradenú licenciu na SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b8ce3-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="b8ce3-106">Novovytvorené kontá priradené k licencii na SharePoint alebo role správcu sa môžu vyskytnúť problémy pri prístupe k SharePointu, ako je napríklad "prístup odmietnutý" alebo "používateľ sa nenašiel".</span><span class="sxs-lookup"><span data-stu-id="b8ce3-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="b8ce3-107">Dajte aspoň 24 hodín na dokončenie synchronizácie vo všetkých našich systémoch.</span><span class="sxs-lookup"><span data-stu-id="b8ce3-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="b8ce3-108">Chápeme, že 24 hodín sa môže zdať príliš dlhý.</span><span class="sxs-lookup"><span data-stu-id="b8ce3-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="b8ce3-109">V mnohých prípadoch už pracujeme na riešení.</span><span class="sxs-lookup"><span data-stu-id="b8ce3-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="b8ce3-110">Používatelia s oprávnením riadenia identitou[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)môžu získať prístup odmietnutý, ak je časové okno s povoleným prístupom veľmi malé, pozrite si časť Prístup odmietnutý [ku kontám PIM.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="b8ce3-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>