---
title: Povoliť Office 365 ATP pre SharePoint, OneDrive a Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703441"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="090ad-102">Povoliť Office 365 pokročilé ohrozenia ochrany SharePoint Online, OneDrive a Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="090ad-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="090ad-103">Prejdite na https://protection.office.com a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="090ad-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="090ad-104">Vyberte položku**politika** >  **správy** > hrozieb**bezpečné prílohy**.</span><span class="sxs-lookup"><span data-stu-id="090ad-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="090ad-105">Vyberte možnosť **Zapnúť ATP pre SharePoint, OneDrive a Microsoft teams**a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="090ad-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="090ad-106">Odporúča Ako globálny správca alebo SharePoint Online správca, spustite rutinu cmdlet [set-Sponájomcu](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **Disallowinfectedfiledownload** nastavená na *hodnotu True*.</span><span class="sxs-lookup"><span data-stu-id="090ad-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="090ad-107">Odporúča [Nastavte výstrahy pre rozpoznané](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) súbory.</span><span class="sxs-lookup"><span data-stu-id="090ad-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="090ad-108">ATP bude nAk chcete skenovať každý súbor v SharePointe Online, OneDrive alebo Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="090ad-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="090ad-109">Súbory sa skenujú asynchrónne, a to prostredníctvom procesu, ktorý používa akcie zdieľania a hosťovskej aktivity spolu s inteligentnými heuristami a signálmi hrozieb na identifikáciu škodlivých súborov.</span><span class="sxs-lookup"><span data-stu-id="090ad-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="090ad-110">Vidieť [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="090ad-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>