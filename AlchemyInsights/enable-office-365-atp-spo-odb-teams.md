---
title: Povolenie protokolu ATP služieb Office 365 pre SharePoint, OneDrive a Microsoft Teams
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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506933"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="74c04-102">Povolenie rozšírenej ochrany pred hrozbami služieb Office 365 pre SharePoint Online, OneDrive a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="74c04-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="74c04-103">Choď te https://protection.office.com do a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="74c04-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="74c04-104">Vyberte položku **Threat management**Policy Safe Attachments (Bezpečné prílohy politiky správy  >  **Policy**  >  **hrozieb).**</span><span class="sxs-lookup"><span data-stu-id="74c04-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="74c04-105">Vyberte položku **Zapnúť atp pre SharePoint, OneDrive a Microsoft Teams a**potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="74c04-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="74c04-106">(Odporúča sa) Ako globálny správca alebo správca SharePointu Online spustite rutinu cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** nastaveným na *hodnotu true*.</span><span class="sxs-lookup"><span data-stu-id="74c04-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="74c04-107">(Odporúča sa) [Nastavte upozornenia](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) na zistené súbory.</span><span class="sxs-lookup"><span data-stu-id="74c04-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="74c04-108">ATP bude skenovať každý jeden súbor v SharePointE Online, OneDrive alebo Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="74c04-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="74c04-109">Súbory sa kontrolujú asynchrónne prostredníctvom procesu, ktorý používa udalosti zdieľania a aktivity hostí spolu s inteligentnou heuristikou a signálmi hrozieb na identifikáciu škodlivých súborov.</span><span class="sxs-lookup"><span data-stu-id="74c04-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="74c04-110">Pozrite [si tému ATP pre SharePoint, OneDrive a Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="74c04-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>