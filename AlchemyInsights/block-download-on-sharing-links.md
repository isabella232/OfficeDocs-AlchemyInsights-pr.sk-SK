---
title: Blokovať preberanie na zdieľanie prepojení
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358515"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="8e6c5-102">Blokovať preberanie na zdieľanie prepojení</span><span class="sxs-lookup"><span data-stu-id="8e6c5-102">Block download on sharing links</span></span>

<span data-ttu-id="8e6c5-103">**Blokovať preberanie** je k dispozícii pre **odkazy iba na zobrazenie** na dokumenty balíka Office.</span><span class="sxs-lookup"><span data-stu-id="8e6c5-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="8e6c5-104">Keď vyberiete túto možnosť, ľudia, ktorí získajú prístup k súboru prostredníctvom odkazu, ktorý ste vytvorili, nebudú vidieť možnosti na prevzatie, tlač alebo kopírovanie súboru.</span><span class="sxs-lookup"><span data-stu-id="8e6c5-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="8e6c5-105">Správcovia môžu kontrolovať, či sa nastavenie "Blokovať preberanie" zobrazí len pre súbory balíka Office alebo nie zmenou `BlockDownloadLinksFileType` nastavenia rutiny cmdlet [set-sponájomcu](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) alebo [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8e6c5-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
