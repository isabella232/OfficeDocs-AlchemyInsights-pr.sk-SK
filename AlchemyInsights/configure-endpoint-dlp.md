---
title: Konfigurovať DLP koncového bodu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402453"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="9ab2e-102">Konfigurovať DLP koncového bodu</span><span class="sxs-lookup"><span data-stu-id="9ab2e-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="9ab2e-103">Microsoft Endpoint DLP umožňuje rozšíriť ochranu pred únikom údajov a možnosti monitorovania na citlivé informácie v zariadeniach s Windowsom 10.</span><span class="sxs-lookup"><span data-stu-id="9ab2e-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="9ab2e-104">Po zaradení zariadení do správy zariadení môžete vytvoriť politiky DLP na vynútenie ochranných akcií pre položky.</span><span class="sxs-lookup"><span data-stu-id="9ab2e-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="9ab2e-105">Prieskumník aktivít možno použiť na monitorovanie citlivých položiek v aktivite.</span><span class="sxs-lookup"><span data-stu-id="9ab2e-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="9ab2e-106">Ďalšie informácie nájdete v téme [Zaradenie zariadení do správy zariadení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="9ab2e-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="9ab2e-107">Ak chcete začať pracovať s DLP koncového bodu:</span><span class="sxs-lookup"><span data-stu-id="9ab2e-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="9ab2e-108">Skontrolujte, či máte príslušné licencie na jednotku SKU/predplatné.</span><span class="sxs-lookup"><span data-stu-id="9ab2e-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="9ab2e-109">Ďalšie informácie nájdete v téme [Licencie na jednotku SKU/predplatné](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="9ab2e-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="9ab2e-110">Skontrolujte povolenia potrebné na povolenie správy zariadení, prístup na stránku zaradenia alebo zapnutie alebo vypnutie monitorovania zariadenia.</span><span class="sxs-lookup"><span data-stu-id="9ab2e-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="9ab2e-111">Ďalšie informácie nájdete v téme [Povolenia](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="9ab2e-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="9ab2e-112">Zaraďte zariadenia do Správy zariadení pomocou postupu na zaradenie zariadení.</span><span class="sxs-lookup"><span data-stu-id="9ab2e-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="9ab2e-113">Ak v časti **Nastavenia** dodržiavania súladu pre M365 chýba možnosť Zaradenie zariadenia (ukážka), skontrolujte, či máte príslušnú licenciu a povolenia uvedené vyššie.</span><span class="sxs-lookup"><span data-stu-id="9ab2e-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="9ab2e-114">Ďalšie informácie nájdete v téme [Zaradenie zariadení](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="9ab2e-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="9ab2e-115">Vytvorte politiky DLP na ochranu citlivých položiek.</span><span class="sxs-lookup"><span data-stu-id="9ab2e-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="9ab2e-116">Informácie nájdete v téme [Scenáre politiky DLP koncového bodu](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="9ab2e-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="9ab2e-117">Ďalšie informácie o nástroji Microsoft Endpoint DLP nájdete v téme [Informácie o ochrane pred únikom údajov v koncovom bode pre Microsoft 365 (ukážka)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="9ab2e-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="9ab2e-118">**Dôležité kroky na zhromažďovanie údajov, ak je potrebná podpora:**</span><span class="sxs-lookup"><span data-stu-id="9ab2e-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="9ab2e-119">Stiahnite verziu preview diagnostického nástroja MDATP Client Analyzer z lokality [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="9ab2e-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="9ab2e-120">Spustite nástroj ako správca v okne cmd:</span><span class="sxs-lookup"><span data-stu-id="9ab2e-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="9ab2e-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="9ab2e-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="9ab2e-122">Po zobrazení výzvy „Zadajte počet minút na zhromažďovanie sledovania:“ zadajte počet minút, ktoré sú potrebné na spustenie scenára</span><span class="sxs-lookup"><span data-stu-id="9ab2e-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="9ab2e-123">Spustite scenár</span><span class="sxs-lookup"><span data-stu-id="9ab2e-123">Run the scenario</span></span>

<span data-ttu-id="9ab2e-124">Zhromaždite výstup súboru ZIP, ktorý poskytnete agentovi podpory.</span><span class="sxs-lookup"><span data-stu-id="9ab2e-124">Collect the Zip file output to be given to the Support agent.</span></span>
