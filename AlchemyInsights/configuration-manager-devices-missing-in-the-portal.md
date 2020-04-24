---
title: Na portáli chýbajú zariadenia Správcu konfigurácie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790232"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="16f98-102">Na portáli chýbajú zariadenia Správcu konfigurácie</span><span class="sxs-lookup"><span data-stu-id="16f98-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="16f98-103">Ak chcete, aby synchronizácia zariadenia fungovala, z lokálneho servera hosťujúceho rolu bodu pripojenia služby musia byť dosiahnuteľné [povinné internetové koncové body](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints).</span><span class="sxs-lookup"><span data-stu-id="16f98-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="16f98-104">Ak chcete vyriešiť problém so synchronizáciou zariadenia, pozrite si súbor **CMGatewaySyncUploadWorker.log** nachádzajúci sa na bode pripojenia služby.</span><span class="sxs-lookup"><span data-stu-id="16f98-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="16f98-105">Prečítajte si ďalšie informácie v téme [Priradenie nájomníka pomocou funkcie Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="16f98-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
