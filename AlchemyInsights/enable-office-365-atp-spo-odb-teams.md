---
title: Povoliť Office 365 ATP pre SharePoint a OneDrive Microsoft tímy
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031086"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="ba27d-102">Zapnutie ochrany Office 365 pokročilé hrozby pre SharePoint Online, OneDrive a Microsoft tímy</span><span class="sxs-lookup"><span data-stu-id="ba27d-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="ba27d-103">Prejsť na https://protection.office.com a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="ba27d-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="ba27d-104">Vybrať **Threat management** > **politika** > **Bezpečnými prílohami**.</span><span class="sxs-lookup"><span data-stu-id="ba27d-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="ba27d-105">Vyberte **Zapnúť ATP pre SharePoint, OneDrive, a tímy spoločnosti Microsoft**a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="ba27d-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="ba27d-106">(Odporúča sa) Ako globálny správca alebo správca SharePoint Online, spustite rutinu cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s **DisallowInfectedFileDownload** parameter nastavený na *hodnotu true*.</span><span class="sxs-lookup"><span data-stu-id="ba27d-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="ba27d-107">(Odporúča sa) [Nastaviť upozornenia](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pre rozpoznaných súborov.</span><span class="sxs-lookup"><span data-stu-id="ba27d-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="ba27d-108">ATP sa nto scan každý súbor SharePoint Online, OneDrive alebo Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ba27d-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="ba27d-109">Súbory sú kontrolované asynchrónne, cez proces, ktorý využíva zdieľanie a hodnotenie činnosti udalosti, spolu s smart heuristiky a hrozba signály na identifikáciu škodlivého súborov.</span><span class="sxs-lookup"><span data-stu-id="ba27d-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="ba27d-110">Pozrite si [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="ba27d-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>