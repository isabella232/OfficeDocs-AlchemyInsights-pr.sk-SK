---
title: Riešenie bežných problémov s programom Microsoft Defender pre Office 365
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
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695627"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="4f052-102">Riešenie bežných problémov s programom Microsoft Defender pre Office 365</span><span class="sxs-lookup"><span data-stu-id="4f052-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="4f052-103">Tu je niekoľko riešení bežných problémov s programom Microsoft Defender pre Office 365:</span><span class="sxs-lookup"><span data-stu-id="4f052-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="4f052-104">**Oneskorenie správy:** Ak sa vyskytnú problémy, v ktorých je doručenie správ oneskorené, budete chcieť použiť **Dynamické možnosti doručenia** v rámci politiky bezpečných príloh.</span><span class="sxs-lookup"><span data-stu-id="4f052-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="4f052-105">Ďalšie informácie nájdete v téme [dynamické doručovanie v politikách bezpečných príloh](https://go.microsoft.com/fwlink/?linkid=2094106).</span><span class="sxs-lookup"><span data-stu-id="4f052-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="4f052-106">**Nahlásenie falošných pozitívnych alebo záporných výsledkov:** Nahláste správu spoločnosti Microsoft pomocou tohto prepojenia: [portál odpovedí Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2092835).</span><span class="sxs-lookup"><span data-stu-id="4f052-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="4f052-107">**Povolenie ochrany bezpečného prepojenia:**</span><span class="sxs-lookup"><span data-stu-id="4f052-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="4f052-108">Prihláste sa do [Centra zabezpečenia dodržiavania súladu služieb Office 365 &](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="4f052-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="4f052-109">Prejdite na   >    >  **bezpečné prepojenia** politiky správy hrozieb.</span><span class="sxs-lookup"><span data-stu-id="4f052-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="4f052-110">V časti **politiky, ktoré sa vzťahujú na konkrétnych príjemcov**, otvorte politiku nakonfigurovanú.</span><span class="sxs-lookup"><span data-stu-id="4f052-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="4f052-111">V časti **nastavenia** vyberte položku **použiť bezpečné prepojenia na správy odoslané v rámci organizácie**.</span><span class="sxs-lookup"><span data-stu-id="4f052-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
