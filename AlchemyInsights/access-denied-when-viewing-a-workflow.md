---
title: Prístup odmietnutý pri zobrazení pracovného postupu
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28310842"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="baeea-102">Prístup odmietnutý pri zobrazení pracovného postupu</span><span class="sxs-lookup"><span data-stu-id="baeea-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="baeea-103">Pracovné postupy služby SharePoint 2013, ktoré sa pokúšajú odoslať e-mail do skupiny SharePoint môžu zlyhať s chybové hlásenie "Prístup odmietnutý" Ak členstvo skupiny lokality SharePoint nie je nastavený pre každého.</span><span class="sxs-lookup"><span data-stu-id="baeea-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="baeea-104">**Ak chcete vyriešiť tento problém, postupujte nasledovne:**</span><span class="sxs-lookup"><span data-stu-id="baeea-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="baeea-105">Aby všetci vidieť členom skupiny SharePoint.</span><span class="sxs-lookup"><span data-stu-id="baeea-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="baeea-106">Odstráňte skupinu SharePoint z poľa Komu alebo Kópiazadajte riadok e-mailu.</span><span class="sxs-lookup"><span data-stu-id="baeea-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="baeea-107">Výslovne pridať používateľov do poľa Komu alebo Kópiazadajte Ak členstvo viditeľnosť nemožno zmeniť skupinu lokality SharePoint.</span><span class="sxs-lookup"><span data-stu-id="baeea-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="baeea-108">Zobrazte viac podrobností nájdete [HTTP neoprávnené na /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="baeea-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

