---
title: Diagnostika pre rôzne problémy s prístupom k portom
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036809"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="1d2c3-102">Diagnostika pre rôzne problémy s prístupom k portom</span><span class="sxs-lookup"><span data-stu-id="1d2c3-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="1d2c3-103">Ak chcete vyriešiť rôzne problémy s prístupom k portu, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="1d2c3-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="1d2c3-104">Zastavte alebo oddeľte virtuálny počítač (VM) z portálu, reštartujte VM a otestujte znova.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="1d2c3-105">Skontrolujte nastavenia siete VM a zistite, či máte zablokované prenosy v skupinách zabezpečenia siete (NSGs).</span><span class="sxs-lookup"><span data-stu-id="1d2c3-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="1d2c3-106">Môžete tiež použiť [nástroj na overenie toku IP nástroja Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) na kontrolu NSGs blokovania premávky, User-Defined trás (UDRs) presmeruje prenos späť na lokálne (' predvolená trasa ' 0.0.0.0/0) alebo do sieťového zariadenia.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="1d2c3-107">Ak sa vyskytnú problémy aj po vyskúšaní vyššie uvedených krokov, zadajte názov VM a port TCP, ku ktorému sa pokúšate odoslať poštu na ďalšiu diagnózu.</span><span class="sxs-lookup"><span data-stu-id="1d2c3-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="1d2c3-108">**Odporučené dokumenty**</span><span class="sxs-lookup"><span data-stu-id="1d2c3-108">**Recommended Documents**</span></span>

[<span data-ttu-id="1d2c3-109">Obmedzenia a odporúčania na odosielanie odchádzajúcich e-mailov cez port 25</span><span class="sxs-lookup"><span data-stu-id="1d2c3-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)