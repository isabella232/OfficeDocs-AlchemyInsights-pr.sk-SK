---
title: Prístup odmietnutý pri zobrazení pracovného postupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688817"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="ae8b6-102">Prístup odmietnutý pri zobrazení pracovného postupu</span><span class="sxs-lookup"><span data-stu-id="ae8b6-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="ae8b6-103">Pracovné postupy SharePointu 2013, ktoré sa pokúšajú odoslať e-maily do skupiny SharePointu, môžu zlyhať s chybovým hlásením "prístup odmietnutý", ak členstvo v skupine SharePoint nie je nastavené na hodnotu všetci.</span><span class="sxs-lookup"><span data-stu-id="ae8b6-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="ae8b6-104">**Ak chcete tento problém vyriešiť, vykonajte tieto kroky:**</span><span class="sxs-lookup"><span data-stu-id="ae8b6-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="ae8b6-105">Povoliť každému Zobraziť členov skupiny SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ae8b6-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="ae8b6-106">Odstráňte skupinu SharePointu z riadku Komu alebo kópia e-mailu.</span><span class="sxs-lookup"><span data-stu-id="ae8b6-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="ae8b6-107">Ak nie je možné zmeniť viditeľnosť členstva v skupine SharePoint, explicitne Pridajte používateľov do riadku Komu alebo kópia.</span><span class="sxs-lookup"><span data-stu-id="ae8b6-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="ae8b6-108">Ak chcete zobraziť ďalšie podrobnosti, prečítajte si [http neoprávnené na/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="ae8b6-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  