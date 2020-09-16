---
title: Riešenie problémov s výkonom služby OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757900"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="38ed6-102">Riešenie problémov s výkonom služby OneDrive</span><span class="sxs-lookup"><span data-stu-id="38ed6-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="38ed6-103">Ak sa vyskytuje pomalší než očakávaná synchronizácia alebo podobné problémy s výkonom vo OneDrive:</span><span class="sxs-lookup"><span data-stu-id="38ed6-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="38ed6-104">Skontrolujte, či nie sú známe žiadne problémy s použitím [tabule stavu služby](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="38ed6-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="38ed6-105">[Povoliť súbory na požiadanie](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , aby ste mali prístup k všetkým súborom vo OneDrive bez nutnosti sťahovania všetkých súborov a použitia ukladacieho priestoru vo vašom zariadení.</span><span class="sxs-lookup"><span data-stu-id="38ed6-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="38ed6-106">[Pozrite si najvhodnejšie postupy](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) pri plánovaní a výkone siete.</span><span class="sxs-lookup"><span data-stu-id="38ed6-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="38ed6-107">[Maximalizujte rýchlosť nahrávania a sťahovania](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), najmä ak synchronizujete zariadenie prvýkrát.</span><span class="sxs-lookup"><span data-stu-id="38ed6-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="38ed6-108">Ak synchronizujete knižnicu s viac než 100 000 položkami, synchronizácia OneDrivu sa môže zdať dlhšiu dobu alebo stav zobrazuje spracovanie 0KB xMB.</span><span class="sxs-lookup"><span data-stu-id="38ed6-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="38ed6-109">[Získajte ďalšie informácie o synchronizácii viac než 100 000 súborov](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , ako aj [podporovaného limitu pre súbory 300 000 v službe OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="38ed6-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="38ed6-110">Keď používateľ prekročí limity používania, SharePoint Online obmedzí všetky ďalšie požiadavky tohto používateľského konta na krátke obdobie.</span><span class="sxs-lookup"><span data-stu-id="38ed6-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="38ed6-111">Všetky akcie používateľov sú obmedzené, kým je plyn v platnosti.</span><span class="sxs-lookup"><span data-stu-id="38ed6-111">All user actions are throttled while the throttle is in effect.</span></span>
