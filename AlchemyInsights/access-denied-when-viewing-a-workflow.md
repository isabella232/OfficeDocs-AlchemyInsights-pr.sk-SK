---
title: Prístup bol odmietnutý pri prezeraní pracovného postupu
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747763"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="d8382-102">Prístup bol odmietnutý pri prezeraní pracovného postupu</span><span class="sxs-lookup"><span data-stu-id="d8382-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="d8382-103">SharePoint 2013 toky činností, ktoré sa pokúšajú odoslať e-mail skupiny SharePoint môže zlyhať s "prístup odmietnutý" chybové hlásenie, ak členstvo v skupine SharePoint nie je nastavená na všetky.</span><span class="sxs-lookup"><span data-stu-id="d8382-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="d8382-104">**Ak chcete vyriešiť tento problém, postupujte nasledovne:**</span><span class="sxs-lookup"><span data-stu-id="d8382-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="d8382-105">Umožním všetkým vidieť členov skupiny SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d8382-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="d8382-106">Odstráňte skupinu SharePoint z riadka Komu alebo kópia e-mailu.</span><span class="sxs-lookup"><span data-stu-id="d8382-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="d8382-107">Explicitne pridať používateľov do riadka Komu alebo kópia, ak nie je možné zmeniť členstvo viditeľnosť pre skupinu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d8382-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="d8382-108">Ak chcete zobraziť ďalšie podrobnosti nájdete [http neoprávnené/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="d8382-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  