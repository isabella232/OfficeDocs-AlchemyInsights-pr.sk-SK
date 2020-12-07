---
title: Čo robiť, ak funkcie Azure v prehliadači Microsoft Edge nefungujú správne
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583783"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="c6416-102">Čo robiť, ak funkcie Azure v prehliadači Microsoft Edge nefungujú správne</span><span class="sxs-lookup"><span data-stu-id="c6416-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="c6416-103">Microsoft Edge obsahuje [známe problémy](https://go.microsoft.com/fwlink/?linkid=2140608) týkajúce sa zón zabezpečenia a môže ovplyvniť spôsob prihlasovania používateľov služby Azure do centra spravovania pre Windows.</span><span class="sxs-lookup"><span data-stu-id="c6416-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="c6416-104">Ak máte problémy s používaním funkcií Azure v prehliadači Microsoft Edge, vyskúšajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="c6416-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="c6416-105">V ponuke **Štart** vyhľadajte položku **Možnosti siete Internet** a vyberte ju.</span><span class="sxs-lookup"><span data-stu-id="c6416-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="c6416-106">V dialógovom okne **Vlastnosti siete Internet** prejdite na kartu **zabezpečenie** .</span><span class="sxs-lookup"><span data-stu-id="c6416-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="c6416-107">Vyberte zónu **Dôveryhodné lokality** a potom kliknite na tlačidlo **lokality** .</span><span class="sxs-lookup"><span data-stu-id="c6416-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="c6416-108">V dialógovom okne **Dôveryhodné lokality** pridajte URL adresu brány, ako aj [https://login.microsoftonline.com](https://login.microsoftonline.com) a [https://login.live.com](https://login.live.com) potom vyberte položku **zatvorenie**.</span><span class="sxs-lookup"><span data-stu-id="c6416-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="c6416-109">V dialógovom okne **Vlastnosti siete Internet** prejdite na kartu **Ochrana osobných údajov** .</span><span class="sxs-lookup"><span data-stu-id="c6416-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="c6416-110">V časti **Blokovanie automaticky otváraných okien** vyberte položku **nastavenia**.</span><span class="sxs-lookup"><span data-stu-id="c6416-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="c6416-111">V dialógovom okne, ktoré sa otvorí, pridajte URL adresu brány, ako aj [https://login.microsoftonline.com](https://login.microsoftonline.com) a [https://login.live.com](https://login.live.com) potom vyberte položku **zatvorenie**.</span><span class="sxs-lookup"><span data-stu-id="c6416-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
