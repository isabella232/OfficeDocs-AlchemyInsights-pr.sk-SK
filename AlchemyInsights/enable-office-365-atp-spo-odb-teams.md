---
title: Povoľte Office 365 ATP pre SharePoint, OneDrive a Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543943"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="17f43-102">Povoľte Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="17f43-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="17f43-103">Prejdite na https://protection.office.com položku a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="17f43-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="17f43-104">Vyberte **položku Politika správy**  >  **hrozieb** Trezor  >  **prílohy**.</span><span class="sxs-lookup"><span data-stu-id="17f43-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="17f43-105">Vyberte **položku Zapnúť Defender for Office 365 pre SharePoint, OneDrive a Microsoft Teams** a potom kliknite na položku **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="17f43-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="17f43-106">(Odporúča sa) Ako globálny správca alebo správca služby SharePoint Online spustite rutinu typu cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** nastaveným na *hodnotu true.*</span><span class="sxs-lookup"><span data-stu-id="17f43-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="17f43-107">(Odporúča sa) [Nastavenie upozornení pre](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) zistené súbory.</span><span class="sxs-lookup"><span data-stu-id="17f43-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="17f43-108">Microsoft Defender pre Office 365 nebude kontrolovať každý súbor v SharePoint Online, OneDrive alebo Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="17f43-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="17f43-109">Súbory sa naskenujú asynchrónne, a to procesom, ktorý využíva udalosti zdieľania a aktivity hostí, ako aj inteligentné heuštie a signály hrozieb na identifikáciu škodlivých súborov.</span><span class="sxs-lookup"><span data-stu-id="17f43-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="17f43-110">Pozrite [si časť Microsoft Defender Office 365 pre SharePoint, OneDrive a Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="17f43-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>