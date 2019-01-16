---
title: Synchronizácie profilu
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311152"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="1e6b8-102">Keď môj profil zmeny synchronizovať SharePoint používateľa profil aplikácie?</span><span class="sxs-lookup"><span data-stu-id="1e6b8-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="1e6b8-103">SharePoint Online používa Active Directory Import časovača (AD Import) importovať používateľov a skupín do aplikácie používateľského profilu.</span><span class="sxs-lookup"><span data-stu-id="1e6b8-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="1e6b8-p101">AD Import synchronizuje zmeny z lokality SharePoint Online adresár Store aplikácie používateľského profilu. Tieto zmeny sú spracované v dávkach.</span><span class="sxs-lookup"><span data-stu-id="1e6b8-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="1e6b8-106">Úloha časovača beží, kým sa zmeny nesynchronizujú.</span><span class="sxs-lookup"><span data-stu-id="1e6b8-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="1e6b8-p102">Čase, keď sa má spustiť úloha závisí od počtu zmien spracovať. Veľký počet zmien trvá dlhšie. Service Level Agreement (SLA) uvádza, že zmena používateľa v adresári služby SharePoint Online sa prejaví v aplikácii používateľského profilu v 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="1e6b8-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="1e6b8-110">Viac informácií o synchronizácia používateľského profilu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1e6b8-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

