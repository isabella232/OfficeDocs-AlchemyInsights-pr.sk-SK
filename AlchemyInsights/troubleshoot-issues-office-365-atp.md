---
title: Riešenie problémov s balíkom Office 365 Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758080"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="107b0-102">Riešenie problémov s balíkom Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="107b0-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="107b0-103">**Všimnite si meškania s doručením e-mailových správ**?</span><span class="sxs-lookup"><span data-stu-id="107b0-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="107b0-104">Skúste použiť možnosť dynamické doručenie pre politiky v oblasti bezpečnosti príloh ATP.</span><span class="sxs-lookup"><span data-stu-id="107b0-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="107b0-105">Týmto sa vyhnete meškaniu doručovania e-mailových správ a zároveň chránite príjemcov pred škodlivými súbormi.</span><span class="sxs-lookup"><span data-stu-id="107b0-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="107b0-106">**Chcete nahlásiť falošné pozitíva alebo falošné negatívy**?</span><span class="sxs-lookup"><span data-stu-id="107b0-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="107b0-107">Pomocou tohto prepojenia odošlete súbor na analýzu: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="107b0-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="107b0-108">Vedeli **ste, že môžete povoliť ochranu zabezpečených prepojení ATP v e-mailoch odoslaných medzi ľuďmi vo vašej organizácii**?</span><span class="sxs-lookup"><span data-stu-id="107b0-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="107b0-109">Vykonajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="107b0-109">Follow these steps:</span></span>
    1. <span data-ttu-id="107b0-110">Prejdite na https://protection.office.com položku a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="107b0-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="107b0-111">Prejdite na **Threat management**  >  **Policy**  >  **bezpečné prepojenia**politiky správy hrozieb.</span><span class="sxs-lookup"><span data-stu-id="107b0-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="107b0-112">V časti **politiky, ktoré sa vzťahujú na konkrétnych príjemcov**, upravte (alebo pridajte) politiku.</span><span class="sxs-lookup"><span data-stu-id="107b0-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="107b0-113">Vyberte položku **použiť bezpečné prepojenia na správy odoslané v rámci organizácie**.</span><span class="sxs-lookup"><span data-stu-id="107b0-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="107b0-114">Uložte si politiku a počkajte 30 minút, kým sa vaše zmeny budú môcť používať v údajovom centre.</span><span class="sxs-lookup"><span data-stu-id="107b0-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="107b0-115">Ak chcete získať ďalšiu pomoc s ATP, pozrite si tému [Ochrana pred rozšírenou hrozbou pre Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="107b0-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>