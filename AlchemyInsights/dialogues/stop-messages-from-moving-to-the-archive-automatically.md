---
title: Zastavenie automatického premiestnenia správ do archívu
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527115"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="f41fa-102">Zastavenie automatického premiestnenia správ do archívu</span><span class="sxs-lookup"><span data-stu-id="f41fa-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="f41fa-103">Ak používate politiku uchovávania údajov, môžete v tejto politike zmeniť vek uchovávania údajov, aby sa správy automaticky nearchivovali.</span><span class="sxs-lookup"><span data-stu-id="f41fa-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="f41fa-104">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="f41fa-104">Here's how:</span></span>

1. <span data-ttu-id="f41fa-105">V [centre spravovania pre Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)vyberte položku značky uchovávania údajov **manažmentu súladu**  >  .</span><span class="sxs-lookup"><span data-stu-id="f41fa-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="f41fa-106">Vyhľadajte značku uchovávania údajov na archiváciu.</span><span class="sxs-lookup"><span data-stu-id="f41fa-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="f41fa-107">V značke uchovávania údajov zmeňte obdobie uchovávania (obdobie archivácie), aby ste **nikdy** nezastavili automatické archivovanie položiek pomocou politiky uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="f41fa-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="f41fa-108">Týmto sa zmení nastavenie archivácie pre všetky poštové schránky s použitím tejto značky uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="f41fa-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
