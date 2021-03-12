---
title: Množina replík
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714590"
---
# <a name="replica-set"></a><span data-ttu-id="83ca1-102">Množina replík</span><span class="sxs-lookup"><span data-stu-id="83ca1-102">Replica set</span></span>

<span data-ttu-id="83ca1-103">AADDS sa nazýva aj spravovaná doména.</span><span class="sxs-lookup"><span data-stu-id="83ca1-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="83ca1-104">Je to vlastne dva radiče domén, ktoré sú spustené a udržiavané backendom.</span><span class="sxs-lookup"><span data-stu-id="83ca1-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="83ca1-105">Dva radiče domén zahŕňajú jednu hlavnú DC a jednu replikáciu DC.</span><span class="sxs-lookup"><span data-stu-id="83ca1-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="83ca1-106">Zálohy v AADDS (spravovaná doména) sú automatizovaný proces spravovaný platformou Azure.</span><span class="sxs-lookup"><span data-stu-id="83ca1-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="83ca1-107">V prípade problému s spravovanou doménou vám môže podpora Azure pomôcť pri obnove zo zálohy.</span><span class="sxs-lookup"><span data-stu-id="83ca1-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="83ca1-108">Vytvoríte každú skupinu replík vo virtuálnej sieti.</span><span class="sxs-lookup"><span data-stu-id="83ca1-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="83ca1-109">Každá virtuálna sieť musí byť prispôsobená každej inej virtuálnej sieti, ktorá je hostiteľom množiny replík spravovanej domény.</span><span class="sxs-lookup"><span data-stu-id="83ca1-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="83ca1-110">V tejto konfigurácii sa vytvorí Topológia siete Mesh, ktorá podporuje replikáciu adresárov.</span><span class="sxs-lookup"><span data-stu-id="83ca1-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="83ca1-111">Virtuálna sieť môže podporovať viacero množín replík za predpokladu, že každá množina replík je v inej virtuálnej podsieti.</span><span class="sxs-lookup"><span data-stu-id="83ca1-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="83ca1-112">Ďalšie podrobnosti o skupine replík nájdete v téme [množiny replík konceptov](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="83ca1-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
