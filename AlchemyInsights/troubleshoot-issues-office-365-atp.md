---
title: Riešenie problémov s aplikáciou Microsoft Defender pre Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801422"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="4a455-102">Riešenie problémov s balíkom Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="4a455-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="4a455-103">**Všimnite si meškania s doručením e-mailových správ** ?</span><span class="sxs-lookup"><span data-stu-id="4a455-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="4a455-104">Skúste použiť možnosť dynamické doručenie pre politiky v oblasti bezpečnosti príloh ATP.</span><span class="sxs-lookup"><span data-stu-id="4a455-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="4a455-105">Týmto sa vyhnete meškaniu doručovania e-mailových správ a zároveň chránite príjemcov pred škodlivými súbormi.</span><span class="sxs-lookup"><span data-stu-id="4a455-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="4a455-106">**Chcete nahlásiť falošné pozitíva alebo falošné negatívy** ?</span><span class="sxs-lookup"><span data-stu-id="4a455-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="4a455-107">Pomocou tohto prepojenia odošlete súbor na analýzu: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="4a455-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="4a455-108">Vedeli **ste, že môžete povoliť ochranu zabezpečených prepojení ATP v e-mailoch odoslaných medzi ľuďmi vo vašej organizácii** ?</span><span class="sxs-lookup"><span data-stu-id="4a455-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="4a455-109">Vykonajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="4a455-109">Follow these steps:</span></span>
    1. <span data-ttu-id="4a455-110">Prejdite na https://protection.office.com položku a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="4a455-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="4a455-111">Prejdite na **Threat management**  >  **Policy**  >  **bezpečné prepojenia** politiky správy hrozieb.</span><span class="sxs-lookup"><span data-stu-id="4a455-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="4a455-112">V časti **politiky, ktoré sa vzťahujú na konkrétnych príjemcov** , upravte (alebo pridajte) politiku.</span><span class="sxs-lookup"><span data-stu-id="4a455-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="4a455-113">Vyberte položku **použiť bezpečné prepojenia na správy odoslané v rámci organizácie** .</span><span class="sxs-lookup"><span data-stu-id="4a455-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="4a455-114">Uložte si politiku a počkajte 30 minút, kým sa vaše zmeny budú môcť používať v údajovom centre.</span><span class="sxs-lookup"><span data-stu-id="4a455-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="4a455-115">Ak chcete získať ďalšiu pomoc s ATP, pozrite si tému [Microsoft Defender pre Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="4a455-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>