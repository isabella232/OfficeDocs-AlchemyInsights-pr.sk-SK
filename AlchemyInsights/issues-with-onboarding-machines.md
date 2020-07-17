---
title: Problémy s onboarding stroje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141660"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="0a09c-102">Problémy s onboarding stroje</span><span class="sxs-lookup"><span data-stu-id="0a09c-102">Issues with onboarding machines</span></span>

<span data-ttu-id="0a09c-103">Môžete mať problémy s onboarding stroje mdatp služby.</span><span class="sxs-lookup"><span data-stu-id="0a09c-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="0a09c-104">Ak máte prístup k počítaču koncového používateľa, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="0a09c-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="0a09c-105">Prevezmite diagnostický nástroj [Client Connectivity Analyzer.](https://aka.ms/mdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="0a09c-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="0a09c-106">Extrahujte a spustite MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="0a09c-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="0a09c-107">Vyhľadajte diagnostický denník v priečinku s názvom MDATPClientAnalyzerResult, rovnaký priečinok, kde je prevzatý nástroj Analyzer.</span><span class="sxs-lookup"><span data-stu-id="0a09c-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="0a09c-108">Skontrolujte súbor denníka, MDATPClientAnalyzer.txt, nájsť problémy s nastavením pripojenia alebo internetového servera proxy.</span><span class="sxs-lookup"><span data-stu-id="0a09c-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>