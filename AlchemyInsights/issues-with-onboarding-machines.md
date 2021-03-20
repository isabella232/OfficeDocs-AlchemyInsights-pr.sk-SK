---
title: Problémy so zaradením počítačov do služby Microsoft Defender pre koncové bod
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901582"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="205ce-102">Problémy so zaradením počítačov do služby Microsoft Defender pre koncové bod</span><span class="sxs-lookup"><span data-stu-id="205ce-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="205ce-103">Možno budete mať problémy so zaradením zariadení do služby MDE.</span><span class="sxs-lookup"><span data-stu-id="205ce-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="205ce-104">Ak máte prístup k počítaču koncového používateľa, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="205ce-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="205ce-105">Stiahnite najnovšiu verziu preview diagnostického nástroja [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="205ce-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="205ce-106">Kliknite pravým tlačidlom myši na **MDEClientAnalyzer.cmd** a vyberte možnosť Spustiť ako správca.</span><span class="sxs-lookup"><span data-stu-id="205ce-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="205ce-107">Dodržiavajte odporúčania uvedené v **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="205ce-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="205ce-108">Podrobnejšie denníky nájdete v podpriečinku s názvom **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="205ce-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="205ce-109">Ak potrebujete ďalšiu pomoc, kontaktujte [podporu Microsoft Defender pre koncové body](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) a poskytnite jej výsledný súbor MDEClientAnalyzerResult.zip na analýzu.</span><span class="sxs-lookup"><span data-stu-id="205ce-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
