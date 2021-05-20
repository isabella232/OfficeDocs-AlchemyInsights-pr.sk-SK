---
title: Microsoft Defender pre Office 365 pre SharePoint, OneDrive a Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543592"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="0dec9-102">Microsoft Defender pre Office 365 pre SharePoint, OneDrive a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0dec9-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="0dec9-103">Ak chcete zapnúť Aplikáciu Microsoft Defender pre Office 365:</span><span class="sxs-lookup"><span data-stu-id="0dec9-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="0dec9-104">Prejdite na [https://protection.office.com](https://protection.office.com) konto globálneho správcu alebo správcu zabezpečenia a prihláste sa s týmto kontom.</span><span class="sxs-lookup"><span data-stu-id="0dec9-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="0dec9-105">Na ľavej navigačnej table v **časti Spravovanie hrozieb** **vyberte** položku Politiky Trezor \> **prílohy**.</span><span class="sxs-lookup"><span data-stu-id="0dec9-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="0dec9-106">Vyberte **položku Zapnúť Defender for Office 365 pre SharePoint, OneDrive a Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="0dec9-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="0dec9-107">[Vytvorte politiku upozornenia na aktivitu a](/microsoft-365/compliance/create-activity-alerts) prijímajte oznámenia v prípade, že nájdeme škodlivé súbory.</span><span class="sxs-lookup"><span data-stu-id="0dec9-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="0dec9-108">Úplné pokyny nájdete v téme [Zapnutie alebo Trezor prílohy pre SharePoint, OneDrive a Microsoft Teams.](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="0dec9-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="0dec9-109">**Poznámka:** Microsoft Defender pre Office 365 predvolene neskenuje každý súbor vo SharePoint Online, OneDrive for Business ani Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0dec9-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="0dec9-110">Súbory sa naskenujú asynchrónne procesom, ktorý využíva aktivity zdieľania, aktivitu hostí a signály hrozieb na identifikáciu škodlivých súborov.</span><span class="sxs-lookup"><span data-stu-id="0dec9-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="0dec9-111">Ďalšie informácie nájdete v [téme Trezor prílohy pre SharePoint, OneDrive a Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="0dec9-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
