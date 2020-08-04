---
title: Konfigurácia dlp koncového bodu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556036"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="d5e92-102">Konfigurácia dlp koncového bodu</span><span class="sxs-lookup"><span data-stu-id="d5e92-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="d5e92-103">Microsoft Endpoint DLP umožňuje rozšíriť ochranu DLP a monitorovanie schopnosti citlivé informácie v zariadeniach so systémom Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d5e92-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="d5e92-104">Po zariadenia sú na palube do správy zariadení, môžete vytvoriť DLP politiky na vynútenie ochranných akcií na položky.</span><span class="sxs-lookup"><span data-stu-id="d5e92-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="d5e92-105">Activity Explorer možno sledovať aktivitu pre citlivé položky.</span><span class="sxs-lookup"><span data-stu-id="d5e92-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="d5e92-106">Ďalšie informácie nájdete v téme [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="d5e92-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="d5e92-107">Ak chcete začať s Endpoint DLP:</span><span class="sxs-lookup"><span data-stu-id="d5e92-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="d5e92-108">Uistite sa, že máte príslušné licencie na SKU/predplatné.</span><span class="sxs-lookup"><span data-stu-id="d5e92-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="d5e92-109">Ďalšie informácie nájdete v téme [Licencovanie SKU/predplatného](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="d5e92-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="d5e92-110">Skontrolujte povolenia potrebné na povolenie správy zariadení, prístup na stránku onboardingu alebo zapnutie/vypnutie monitorovania zariadenia.</span><span class="sxs-lookup"><span data-stu-id="d5e92-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="d5e92-111">Ďalšie informácie nájdete v téme [Povolenia](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="d5e92-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="d5e92-112">Palubné zariadenia do správy zariadení podľa postupu onboarding zariadenia.</span><span class="sxs-lookup"><span data-stu-id="d5e92-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="d5e92-113">Ak vám v časti Nastavenie súladu m365 chýba možnosť Onboarding (ukážka) **zariadenia,** potvrďte, že máte príslušnú licenciu a povolenia uvedené vyššie.</span><span class="sxs-lookup"><span data-stu-id="d5e92-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="d5e92-114">Ďalšie informácie nájdete v téme [Zariadenia na na pravovanie](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="d5e92-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="d5e92-115">Vytvorte politiky DLP na ochranu citlivých položiek.</span><span class="sxs-lookup"><span data-stu-id="d5e92-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="d5e92-116">Informácie nájdete v téme [Scenáre politiky Endpoint DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="d5e92-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="d5e92-117">Ďalšie informácie o Microsoft Endpoint DLP nájdete informácie [o Microsoft 365 Endpoint úniku údajov prevencia (náhľad)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="d5e92-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>