---
title: Na portáli chýbajú zariadenia Správcu konfigurácie
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817259"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="e61ec-102">Na portáli chýbajú zariadenia Správcu konfigurácie</span><span class="sxs-lookup"><span data-stu-id="e61ec-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="e61ec-103">Ak chcete, aby synchronizácia zariadenia fungovala, z lokálneho servera hosťujúceho rolu bodu pripojenia služby musia byť dosiahnuteľné [povinné internetové koncové body](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints).</span><span class="sxs-lookup"><span data-stu-id="e61ec-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="e61ec-104">Ak chcete vyriešiť problém so synchronizáciou zariadenia, pozrite si súbor **CMGatewaySyncUploadWorker.log** nachádzajúci sa na bode pripojenia služby.</span><span class="sxs-lookup"><span data-stu-id="e61ec-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="e61ec-105">Prečítajte si ďalšie informácie v téme [Priradenie nájomníka pomocou funkcie Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="e61ec-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
