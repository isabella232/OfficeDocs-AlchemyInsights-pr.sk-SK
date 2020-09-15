---
title: Synchronizácia profilu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801784"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="d82af-102">Kedy sa zmení môj profil na synchronizáciu s aplikáciou používateľských profilov SharePointu?</span><span class="sxs-lookup"><span data-stu-id="d82af-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="d82af-103">V SharePointe Online sa na importovanie používateľov a skupín do aplikácie používateľského profilu používa úloha časovača importu služby Active Directory (Import reklamy).</span><span class="sxs-lookup"><span data-stu-id="d82af-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="d82af-104">Importovanie reklám synchronizuje zmeny z adresárového obchodu SharePoint Online do aplikácie používateľského profilu.</span><span class="sxs-lookup"><span data-stu-id="d82af-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="d82af-105">Tieto zmeny sa spracúvajú v dávkach.</span><span class="sxs-lookup"><span data-stu-id="d82af-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="d82af-106">Úloha časovača sa spustí, až kým sa zmeny nesynchronizujú.</span><span class="sxs-lookup"><span data-stu-id="d82af-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="d82af-107">Časový úsek, v ktorom sa spustí úloha, závisí od počtu zmien, ktoré sa majú spracovať.</span><span class="sxs-lookup"><span data-stu-id="d82af-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="d82af-108">Veľký počet zmien trvá dlhšie.</span><span class="sxs-lookup"><span data-stu-id="d82af-108">A large number of changes takes longer.</span></span> <span data-ttu-id="d82af-109">V zmluve o úrovni služieb (SLA) sa uvádza, že zmeny používateľa v adresári služby SharePoint Online sa prejavia v aplikácii používateľského profilu v priebehu 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="d82af-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="d82af-110">Ďalšie informácie o synchronizácii používateľských profilov v SharePointe Online</span><span class="sxs-lookup"><span data-stu-id="d82af-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

