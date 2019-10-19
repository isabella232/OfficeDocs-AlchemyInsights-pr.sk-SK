---
title: Synchronizácia profilu
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554348"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="772ff-102">Kedy sa môj profil zmení na synchronizáciu s aplikáciou používateľského profilu služby SharePoint?</span><span class="sxs-lookup"><span data-stu-id="772ff-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="772ff-103">SharePoint Online používa Active Directory import časovač prácu (AD Import) importovať používateľov a skupín do aplikácie používateľského profilu.</span><span class="sxs-lookup"><span data-stu-id="772ff-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="772ff-104">AD Import synchronizuje zmeny z lokality SharePoint Online Directory Store do aplikácie používateľského profilu.</span><span class="sxs-lookup"><span data-stu-id="772ff-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="772ff-105">Tieto zmeny sa spracúvajú v dávkach.</span><span class="sxs-lookup"><span data-stu-id="772ff-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="772ff-106">Úloha časovača sa spustí, kým sa zmeny nesynchronizujú.</span><span class="sxs-lookup"><span data-stu-id="772ff-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="772ff-107">Čas potrebný na spustenie úlohy závisí od počtu zmien, ktoré sa majú spracovať.</span><span class="sxs-lookup"><span data-stu-id="772ff-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="772ff-108">Veľké množstvo zmien trvá dlhšie.</span><span class="sxs-lookup"><span data-stu-id="772ff-108">A large number of changes takes longer.</span></span> <span data-ttu-id="772ff-109">Zmluva o úrovni služieb (SLA) uvádza, že zmena používateľa v adresári SharePoint Online sa prejaví v aplikácii používateľského profilu v 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="772ff-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="772ff-110">Ďalšie informácie o synchronizácii používateľského profilu v SharePointe Online</span><span class="sxs-lookup"><span data-stu-id="772ff-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

