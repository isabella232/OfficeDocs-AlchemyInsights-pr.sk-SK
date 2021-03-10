---
title: Deadaptácii mimo zariadenia s Windowsom v programe Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695159"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="0084b-102">Deadaptácii mimo zariadenia s Windowsom v programe Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="0084b-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="0084b-103">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="0084b-103">Here's how:</span></span>

1. <span data-ttu-id="0084b-104">Postupujte podľa dokumentácie tretej strany na odpojenie riešenia tretej strany od spoločnosti Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="0084b-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="0084b-105">Z nájomníka služby Azure Active Directory odstráňte povolenia pre riešenie tretej strany:</span><span class="sxs-lookup"><span data-stu-id="0084b-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="0084b-106">Prihláste sa na [portáli Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="0084b-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="0084b-107">Vyberte položku **všetky služby**  >  **Azure Active Directory**  >  **Enterprise Applications**.</span><span class="sxs-lookup"><span data-stu-id="0084b-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="0084b-108">Vyberte aplikáciu, ktorú chcete deadaptácii.</span><span class="sxs-lookup"><span data-stu-id="0084b-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="0084b-109">Vyberte položku **odstrániť**.</span><span class="sxs-lookup"><span data-stu-id="0084b-109">Select **Delete**.</span></span>

<span data-ttu-id="0084b-110">Ďalšie informácie nájdete v téme [deadaptácii zariadenia mimo Windowsu](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="0084b-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
