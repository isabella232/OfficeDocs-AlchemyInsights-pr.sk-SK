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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657944"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="a11ed-102">Konfigurovať DLP koncového bodu</span><span class="sxs-lookup"><span data-stu-id="a11ed-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="a11ed-103">Microsoft Endpoint DLP umožňuje rozšíriť ochranu pred únikom údajov a možnosti monitorovania na citlivé informácie v zariadeniach s Windowsom 10.</span><span class="sxs-lookup"><span data-stu-id="a11ed-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="a11ed-104">Po zaradení zariadení do správy zariadení môžete vytvoriť politiky DLP na vynútenie ochranných akcií pre položky.</span><span class="sxs-lookup"><span data-stu-id="a11ed-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="a11ed-105">Prieskumník aktivít možno použiť na monitorovanie citlivých položiek v aktivite.</span><span class="sxs-lookup"><span data-stu-id="a11ed-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="a11ed-106">Ďalšie informácie nájdete v téme [Zaradenie zariadení do správy zariadení](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="a11ed-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="a11ed-107">Ak chcete začať pracovať s DLP koncového bodu:</span><span class="sxs-lookup"><span data-stu-id="a11ed-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="a11ed-108">Skontrolujte, či máte príslušné licencie na jednotku SKU/predplatné.</span><span class="sxs-lookup"><span data-stu-id="a11ed-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="a11ed-109">Ďalšie informácie nájdete v téme [Licencie na jednotku SKU/predplatné](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="a11ed-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="a11ed-110">Skontrolujte povolenia potrebné na povolenie správy zariadení, prístup na stránku zaradenia alebo zapnutie alebo vypnutie monitorovania zariadenia.</span><span class="sxs-lookup"><span data-stu-id="a11ed-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="a11ed-111">Ďalšie informácie nájdete v téme [Povolenia](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="a11ed-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="a11ed-112">Zaraďte zariadenia do Správy zariadení pomocou postupu na zaradenie zariadení.</span><span class="sxs-lookup"><span data-stu-id="a11ed-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="a11ed-113">Ďalšie informácie nájdete v téme [Zaradenie zariadení](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="a11ed-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="a11ed-114">Vytvorte politiky DLP na ochranu citlivých položiek.</span><span class="sxs-lookup"><span data-stu-id="a11ed-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="a11ed-115">Informácie nájdete v téme [Scenáre politiky DLP koncového bodu](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="a11ed-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="a11ed-116">Ďalšie informácie o nástroji Microsoft Endpoint DLP nájdete v téme [Informácie o ochrane pred únikom údajov v koncovom bode pre Microsoft 365 (ukážka)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="a11ed-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="a11ed-117">**Dôležité kroky na zhromažďovanie údajov, ak je potrebná podpora:**</span><span class="sxs-lookup"><span data-stu-id="a11ed-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="a11ed-118">Stiahnuť [ukážku analýzy klienta MDATP.](https://aka.ms/betamdatpanalyzer)</span><span class="sxs-lookup"><span data-stu-id="a11ed-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="a11ed-119">Spustite nástroj ako správca v okne cmd:</span><span class="sxs-lookup"><span data-stu-id="a11ed-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="a11ed-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="a11ed-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="a11ed-121">Po zobrazení **výzvy zadajte počet minút** na zhromaždenie sledovania: zadajte počet minút potrebných na spustenie scenára.</span><span class="sxs-lookup"><span data-stu-id="a11ed-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="a11ed-122">Spustite scenár.</span><span class="sxs-lookup"><span data-stu-id="a11ed-122">Run the scenario.</span></span>

<span data-ttu-id="a11ed-123">Zhromaždite výstup súboru zip a dajte ho agentovi podpory.</span><span class="sxs-lookup"><span data-stu-id="a11ed-123">Collect the Zip file output to give to the Support agent.</span></span>
