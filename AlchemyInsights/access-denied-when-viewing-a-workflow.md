---
title: Prístup bol odmietnutý pri prezeraní pracovného postupu
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050540"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="f799f-102">Prístup bol odmietnutý pri prezeraní pracovného postupu</span><span class="sxs-lookup"><span data-stu-id="f799f-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="f799f-103">SharePoint 2013 toky činností, ktoré sa pokúšajú odoslať e-mail skupiny SharePoint môže zlyhať s "prístup odmietnutý" chybové hlásenie, ak členstvo v skupine SharePoint nie je nastavená na všetky.</span><span class="sxs-lookup"><span data-stu-id="f799f-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="f799f-104">**Ak chcete vyriešiť tento problém, postupujte nasledovne:**</span><span class="sxs-lookup"><span data-stu-id="f799f-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="f799f-105">Umožním všetkým vidieť členov skupiny SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f799f-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="f799f-106">Odstráňte skupinu SharePoint z riadka Komu alebo kópia e-mailu.</span><span class="sxs-lookup"><span data-stu-id="f799f-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="f799f-107">Explicitne pridať používateľov do riadka Komu alebo kópia, ak nie je možné zmeniť členstvo viditeľnosť pre skupinu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f799f-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="f799f-108">Ak chcete zobraziť ďalšie podrobnosti nájdete [http neoprávnené na/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="f799f-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  