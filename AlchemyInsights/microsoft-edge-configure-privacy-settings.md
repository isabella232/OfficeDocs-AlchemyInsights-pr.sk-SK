---
title: Konfigurácia nastavenia ochrany osobných údajov v prehliadači Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678859"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="d9d0c-102">Konfigurácia nastavenia ochrany osobných údajov v prehliadači Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d9d0c-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="d9d0c-103">Ak je Microsoft Edge nasadený na platformách iných ako Windows, diagnostické údaje a informácie o lokalite sa na základe predvoleného nastavenia neodosielajú spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d9d0c-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="d9d0c-104">Ak je však Microsoft Edge nasadený vo Windowse 10, diagnostické údaje a informácie o lokalite sa odosielajú v závislosti od [nastavení diagnostických údajov používateľov systému Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="d9d0c-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="d9d0c-105">Ak chcete nakonfigurovať spôsob, akým Microsoft Edge spracuje zhromažďovanie údajov pre vašu organizáciu, použite tieto skupinové politiky:</span><span class="sxs-lookup"><span data-stu-id="d9d0c-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="d9d0c-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Táto politika umožňuje vytváranie hlásení o používaní a údajoch súvisiacich s haváriami.</span><span class="sxs-lookup"><span data-stu-id="d9d0c-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="d9d0c-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Táto politika odošle informácie o lokalite, ktoré sa používajú na zlepšenie služieb spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d9d0c-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="d9d0c-108">Ďalšie informácie nájdete v téme [Konfigurácia nastavenia politiky](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="d9d0c-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>