---
title: Riešenie problémov so službami Office 365 Advanced Threat Protection (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511127"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="e59a8-102">Riešenie problémov s protokolom ATP služieb Office 365</span><span class="sxs-lookup"><span data-stu-id="e59a8-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="e59a8-103">**Oznámenie oneskorenia s doručovanie e-mailových správ?**</span><span class="sxs-lookup"><span data-stu-id="e59a8-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="e59a8-104">Skúste použiť možnosť Dynamické doručovanie pre politiky dôveryhodných príloh ATP.</span><span class="sxs-lookup"><span data-stu-id="e59a8-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="e59a8-105">Tým sa zabráni oneskoreniu doručovania e-mailových správ a zároveň chrániť príjemcov pred škodlivými súbormi.</span><span class="sxs-lookup"><span data-stu-id="e59a8-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="e59a8-106">**Chcete nahlásiť falošne pozitívne alebo falošné negatívy?**</span><span class="sxs-lookup"><span data-stu-id="e59a8-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="e59a8-107">Pomocou tohto prepojenia odošlite súbor na analýzu:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="e59a8-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="e59a8-108">**Vedeli ste, že môžete povoliť ATP Bezpečné odkazy ochranu pre e-mail odoslaný medzi ľuďmi vo vašej organizácii?**</span><span class="sxs-lookup"><span data-stu-id="e59a8-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="e59a8-109">Vykonajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="e59a8-109">Follow these steps:</span></span>
    1. <span data-ttu-id="e59a8-110">Prejdite na https://protection.office.com položku a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="e59a8-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="e59a8-111">Prejdite na **Threat management**  >  **Policy**  >  **Safe Links**.</span><span class="sxs-lookup"><span data-stu-id="e59a8-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="e59a8-112">V časti **Politiky, ktoré sa vzťahujú na konkrétnych príjemcov**, upravte (alebo pridajte) politiku.</span><span class="sxs-lookup"><span data-stu-id="e59a8-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="e59a8-113">Vyberte **položku Použiť bezpečné prepojenia na správy odoslané v rámci organizácie**.</span><span class="sxs-lookup"><span data-stu-id="e59a8-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="e59a8-114">Uložte si pravidlá a nechajte približne 30 minút, aby sa zmeny mohli prejsť cez dátové centrum.</span><span class="sxs-lookup"><span data-stu-id="e59a8-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="e59a8-115">Ak chcete získať ďalšiu pomoc s atp, pozrite si tému [Rozšírená ochrana pred hrozbami služieb Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="e59a8-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>