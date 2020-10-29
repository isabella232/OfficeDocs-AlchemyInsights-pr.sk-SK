---
title: Riešenie problémov s programom Microsoft Defender pre Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801460"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="89c96-102">Riešenie problémov s programom Microsoft Defender pre Office 365</span><span class="sxs-lookup"><span data-stu-id="89c96-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="89c96-103">Všimli ste si oneskorenia v doručovaní správ?</span><span class="sxs-lookup"><span data-stu-id="89c96-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="89c96-104">Použite možnosť [dynamické doručenie](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) v politike bezpečnosti v prílohách ATP.</span><span class="sxs-lookup"><span data-stu-id="89c96-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="89c96-105">To vám pomôže vyhnúť sa oneskoreniu správy a zároveň chrániť príjemcov pred škodlivými súbormi.</span><span class="sxs-lookup"><span data-stu-id="89c96-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="89c96-106">Chcete nahlásiť falošný poplach alebo falošné negatívy spoločnosti Microsoft?</span><span class="sxs-lookup"><span data-stu-id="89c96-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="89c96-107">Pomocou tohto [prepojenia](https://www.microsoft.com/wdsi/filesubmission/) odošlete súbory na analýzu.</span><span class="sxs-lookup"><span data-stu-id="89c96-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="89c96-108">Vedeli ste, že môžete zapnúť ochranu zabezpečených prepojení interných e-mailov odoslaných medzi príjemcami v rámci organizácie?</span><span class="sxs-lookup"><span data-stu-id="89c96-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="89c96-109">Vykonajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="89c96-109">Follow these steps:</span></span>

  1. <span data-ttu-id="89c96-110">Prejdite na [https://protection.office.com](https://protection.office.com) globálneho správcu alebo konto správcu zabezpečenia a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="89c96-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="89c96-111">Na ľavej navigačnej table v časti **Správa hrozieb** vyberte položku **Policy** \> **bezpečné prepojenia** politiky.</span><span class="sxs-lookup"><span data-stu-id="89c96-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="89c96-112">V **politikách, ktoré sa používajú v časti celá organizácia** , vyberte politiku a kliknite na položku **Upraviť** .</span><span class="sxs-lookup"><span data-stu-id="89c96-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="89c96-113">V časti **nastavenia** zapnite **možnosť použiť bezpečné prepojenia na správy odoslané v rámci organizácie** .</span><span class="sxs-lookup"><span data-stu-id="89c96-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
