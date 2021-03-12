---
title: Konfigurovanie a overenie výnimiek pre MDATP v počítači s Linuxom
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749249"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="2aedd-102">Konfigurovanie a overenie výnimiek pre MDATP v počítači s Linuxom</span><span class="sxs-lookup"><span data-stu-id="2aedd-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="2aedd-103">Môžete vylúčiť určité súbory, priečinky, procesy a súbory, ktoré boli otvorené pri spracovaní z MDATP skenov.</span><span class="sxs-lookup"><span data-stu-id="2aedd-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="2aedd-104">Vylúčenia pomáhajú zabrániť nesprávnemu zisťovaniu softvéru a súborov, ktoré sú jedinečné alebo prispôsobené vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="2aedd-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="2aedd-105">Vylúčenie tiež pomáha zmierňovať problémy s výkonom spôsobené MDATP.</span><span class="sxs-lookup"><span data-stu-id="2aedd-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="2aedd-106">Ďalšie informácie nájdete v téme [Konfigurácia a overenie výnimiek pre MDATP pre Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="2aedd-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2aedd-107">Vylúčenia popísané v tomto článku sa netýkajú iných možností MDATP pre Linux vrátane zisťovania koncového bodu a odpovedí (EDR).</span><span class="sxs-lookup"><span data-stu-id="2aedd-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="2aedd-108">Súbory, ktoré vylúčite pomocou metód popísaných v tomto článku, môžu stále vyvolať upozornenia na EDR a ďalšie možnosti zisťovania.</span><span class="sxs-lookup"><span data-stu-id="2aedd-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
