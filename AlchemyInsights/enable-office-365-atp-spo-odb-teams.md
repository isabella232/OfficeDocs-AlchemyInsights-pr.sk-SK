---
title: Povolenie služieb Office 365 ATP pre SharePoint, OneDrive a Microsoft teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709922"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="a1561-102">Povolenie rozšírenej ochrany pred hrozbami pre Office 365 pre SharePoint Online, OneDrive a Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="a1561-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="a1561-103">Prejdite na https://protection.office.com a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="a1561-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="a1561-104">Vyberte **Threat management**  >  **Policy**  >  **bezpečné prílohy**politiky správy hrozieb.</span><span class="sxs-lookup"><span data-stu-id="a1561-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="a1561-105">Vyberte položku **Zapnúť ATP pre SharePoint, OneDrive a Microsoft teams**a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="a1561-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="a1561-106">Odporúča Ako globálny správca alebo správca SharePointu Online spustite rutinu typu cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** nastavený na *hodnotu True*.</span><span class="sxs-lookup"><span data-stu-id="a1561-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="a1561-107">Odporúča [Nastavte upozornenia](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) na zistené súbory.</span><span class="sxs-lookup"><span data-stu-id="a1561-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="a1561-108">ATP bude NAK kontrolovať každý jeden súbor v SharePointe Online, vo OneDrive alebo v aplikácii Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="a1561-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="a1561-109">Súbory sa naskenujú asynchrónne, a to prostredníctvom procesu, ktorý používa akcie zdieľania a aktivity hosťujúcich, spolu s inteligentnou heuristikou a signálmi hrozby na identifikáciu škodlivých súborov.</span><span class="sxs-lookup"><span data-stu-id="a1561-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="a1561-110">Pozrite si tému [ATP pre SharePoint, OneDrive a Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="a1561-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>