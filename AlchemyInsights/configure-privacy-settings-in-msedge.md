---
title: Konfigurácia nastavení ochrany osobných údajov v Microsoft Edgei
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405733"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="e5ff5-102">Konfigurácia nastavení ochrany osobných údajov v Microsoft Edgei</span><span class="sxs-lookup"><span data-stu-id="e5ff5-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="e5ff5-103">Ak je Microsoft Edge nasadený na platformách iných ako Windows, diagnostické údaje a informácie o lokalite sa predvolene spoločnosti Microsoft odosielajú.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="e5ff5-104">Ak je však Microsoft Edge nasadený vo Windowse 10, diagnostické údaje a informácie o lokalite sa odosielajú podľa nastavení diagnostických údajov [systému Windows používateľov.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="e5ff5-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="e5ff5-105">Ak chcete nakonfigurovať, ako Microsoft Edge spracováva zhromažďovanie údajov pre vašu organizáciu, použite tieto skupinové politiky:</span><span class="sxs-lookup"><span data-stu-id="e5ff5-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="e5ff5-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) zapne vykazovanie údajov o používaní a údajoch súvisiacich s zlyhaním.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="e5ff5-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) odosiela informácie o lokalite, ktoré sa používajú na zlepšenie služieb spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e5ff5-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="e5ff5-108">Ďalšie informácie nájdete v téme [Konfigurácia nastavenia politiky.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="e5ff5-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
