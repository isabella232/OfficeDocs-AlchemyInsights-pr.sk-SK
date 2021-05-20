---
title: Riešenie problémov s aplikáciou Microsoft Defender pre Office 365
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
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545283"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="d69e7-102">Riešenie problémov s aplikáciou Microsoft Defender pre Office 365</span><span class="sxs-lookup"><span data-stu-id="d69e7-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="d69e7-103">**Máte oneskorenia pri doručovaní správ?**</span><span class="sxs-lookup"><span data-stu-id="d69e7-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="d69e7-104">Použite možnosť [Dynamické doručovanie](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) v programe Microsoft Defender pre Office 365 Trezor prílohy.</span><span class="sxs-lookup"><span data-stu-id="d69e7-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="d69e7-105">Tým sa predídu oneskoreniam správ a zároveň chránite príjemcov pred škodlivými súbormi.</span><span class="sxs-lookup"><span data-stu-id="d69e7-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="d69e7-106">**Chcete spoločnosti Microsoft nahlásiť nesprávne pozitívne alebo nesprávne negatívy?**</span><span class="sxs-lookup"><span data-stu-id="d69e7-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="d69e7-107">Použite [Prieskumníka odosielania.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="d69e7-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="d69e7-108">-\*\* Vedeli ste, že pre interné e-Trezor odoslané medzi príjemcami vo vašej organizácii môžete povoliť ochranu prepojení na e-mail?\*\* Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="d69e7-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="d69e7-109">Prejdite na [https://protection.office.com](https://protection.office.com) konto globálneho správcu alebo správcu zabezpečenia a prihláste sa s týmto kontom.</span><span class="sxs-lookup"><span data-stu-id="d69e7-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="d69e7-110">Na ľavej navigačnej table v **časti Spravovanie hrozieb** **vyberte** položku Politika Trezor \> **prepojenia**.</span><span class="sxs-lookup"><span data-stu-id="d69e7-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="d69e7-111">V časti **Politiky, ktoré sa vzťahujú na celú organizáciu** vyberte politiku a kliknite na položku **Upraviť**.</span><span class="sxs-lookup"><span data-stu-id="d69e7-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="d69e7-112">V **Nastavenia povoliť** Použitie **bezpečných prepojení na správy odoslané v rámci organizácie.**</span><span class="sxs-lookup"><span data-stu-id="d69e7-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
