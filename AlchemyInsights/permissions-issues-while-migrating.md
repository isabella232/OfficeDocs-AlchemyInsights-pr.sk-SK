---
title: Problémy s povoleniami počas migrácie
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 39b36a85319ccd71278571f3a3cbbc7cf0b9f0fa
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798067"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="de66b-102">Používateľský profil a synchronizácia fotografií</span><span class="sxs-lookup"><span data-stu-id="de66b-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="de66b-103">**Synchronizácia profilových fotografií** – používatelia si môžu všimnúť, že ich profilová fotografia sa nesynchronizuje s lokalitou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="de66b-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="de66b-104">Alebo sa možno pokúsili aktualizovať svoju profilovú fotografiu a fotografia sa stále zobrazuje ako pôvodná fotografia.</span><span class="sxs-lookup"><span data-stu-id="de66b-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="de66b-105">Ak chcete zabezpečiť, aby sa fotografia profilu zobrazovala podľa očakávaní, bude musieť používateľ iniciovať synchronizáciu fotografií.</span><span class="sxs-lookup"><span data-stu-id="de66b-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="de66b-106">Ďalšie informácie o procese synchronizácie fotografií nájdete [v téme informácie o synchronizácii profilových obrázkov v službe Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="de66b-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="de66b-107">**Synchronizácia profilu** – časom, ktorý je potrebný na vykonanie synchronizácie profilu, závisí od počtu zmien (práca), ktorú úloha importu reklamy musí spracovať.</span><span class="sxs-lookup"><span data-stu-id="de66b-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="de66b-108">Ak existuje veľa zmien, úloha časovača má veľa práce a bude trvať dlhšie, kým sa zmeny prejavia v aplikácii používateľského profilu.</span><span class="sxs-lookup"><span data-stu-id="de66b-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="de66b-109">Ak úloha časovača obsahuje malý objem práce, zmeny sa prejavia v aplikácii používateľského profilu oveľa rýchlejšie.</span><span class="sxs-lookup"><span data-stu-id="de66b-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="de66b-110">Ďalšie informácie o procese synchronizácie profilu nájdete [v téme informácie o synchronizácii používateľských profilov v SharePointe Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="de66b-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="de66b-111">**Aktualizácia profilu v balíku Office** – Ponorte používateľov môžete spravovať svoj profil Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="de66b-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="de66b-112">Ďalšie informácie nájdete v téme [zobrazenie a aktualizovanie profilu v Office](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="de66b-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

