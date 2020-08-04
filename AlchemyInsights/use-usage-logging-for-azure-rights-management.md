---
title: Použitie zapisovania do denníka používania pre službu Azure Rights Management
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
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556021"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="19eb4-102">Použitie zapisovania do denníka používania pre službu Azure Rights Management</span><span class="sxs-lookup"><span data-stu-id="19eb4-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="19eb4-103">V predvolenom nastavení je ochrana používania zapisovania do denníka povolené pre všetkých zákazníkov.</span><span class="sxs-lookup"><span data-stu-id="19eb4-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="19eb4-104">Denníky sa zapisujú ako séria objektov blob v azure ukladacieho priestoru nájomcu.</span><span class="sxs-lookup"><span data-stu-id="19eb4-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="19eb4-105">Po operácii ochrany môže trvať až 15 minút, kým sa väčšina denníkov zobrazí.</span><span class="sxs-lookup"><span data-stu-id="19eb4-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="19eb4-106">Denníky používania ochrany môžete použiť na:</span><span class="sxs-lookup"><span data-stu-id="19eb4-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="19eb4-107">Analýza prehľadov podnikov</span><span class="sxs-lookup"><span data-stu-id="19eb4-107">Analyze business insights</span></span>

- <span data-ttu-id="19eb4-108">Monitor na zneužitie</span><span class="sxs-lookup"><span data-stu-id="19eb4-108">Monitor for abuse</span></span>

- <span data-ttu-id="19eb4-109">Vykonanie forenznej analýzy</span><span class="sxs-lookup"><span data-stu-id="19eb4-109">Perform forensic analysis</span></span>

<span data-ttu-id="19eb4-110">Ďalšie informácie sa nachádzajú v [téme Zapisovanie do denníka a analýza ochrany pomocou služby Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span><span class="sxs-lookup"><span data-stu-id="19eb4-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="19eb4-111">Informácie o prihlásení na používanie klienta nájdete v [príručke Správca: Klientske súbory ochrany informácií platformy Azure a zapisovanie do denníka používania klienta](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span><span class="sxs-lookup"><span data-stu-id="19eb4-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="19eb4-112">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="19eb4-112">For additional information, see:</span></span>

- <span data-ttu-id="19eb4-113">[Požiadavky na ochranu informácií služby Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span><span class="sxs-lookup"><span data-stu-id="19eb4-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="19eb4-114">[Kurz: Konfigurácia nastavenia politiky ochrany informácií služby Azure a vytvorenie novej menovky](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span><span class="sxs-lookup"><span data-stu-id="19eb4-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>