---
title: Riešenie problémov s výkonom služby OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733213"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="7bb3a-102">Riešenie problémov s výkonom služby OneDrive</span><span class="sxs-lookup"><span data-stu-id="7bb3a-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="7bb3a-103">Ak sa vyskytnú pomalšie než očakávané synchronizácie alebo podobné problémy s výkonom OneDrive:</span><span class="sxs-lookup"><span data-stu-id="7bb3a-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="7bb3a-104">Potvrďte, že nie sú známe žiadne problémy pomocou [služby Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7bb3a-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="7bb3a-105">[Povoľte súbory na požiadanie](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , aby ste mali prístup k všetkým súborom v službe OneDrive bez nutnosti sťahovať všetky z nich a používať ukladací priestor v zariadení.</span><span class="sxs-lookup"><span data-stu-id="7bb3a-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="7bb3a-106">[Prečítajte si osvedčené postupy](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) pre plánovanie a výkon siete.</span><span class="sxs-lookup"><span data-stu-id="7bb3a-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="7bb3a-107">[Maximalizujte rýchlosť odosielania a preberania](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), najmä ak synchronizujete zariadenie prvýkrát.</span><span class="sxs-lookup"><span data-stu-id="7bb3a-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="7bb3a-108">Ak synchronizujete knižnicu s viac ako 100 000 položkami, OneDrive synchronizácia môže zdať prilepené na dlhú dobu, alebo stav zobrazuje spracovanie 0KB xMB. "</span><span class="sxs-lookup"><span data-stu-id="7bb3a-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="7bb3a-109">Ďalšie [informácie o synchronizácii viac ako 100 000 súborov](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , ako aj [podporovaný limit 300 000 súborov vo OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="7bb3a-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="7bb3a-110">Keď používateľ prekročí limity používania, SharePoint Online throttles akékoľvek ďalšie požiadavky z tohto používateľského konta na krátku dobu.</span><span class="sxs-lookup"><span data-stu-id="7bb3a-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="7bb3a-111">Všetky akcie používateľa sú škrtil, kým škrtiacej klapky je v platnosti.</span><span class="sxs-lookup"><span data-stu-id="7bb3a-111">All user actions are throttled while the throttle is in effect.</span></span>
