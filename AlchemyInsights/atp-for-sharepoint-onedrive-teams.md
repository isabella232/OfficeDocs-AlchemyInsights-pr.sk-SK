---
title: ATP pre SharePoint, OneDrive a Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508427"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="90b99-102">ATP pre SharePoint, OneDrive a Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="90b99-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="90b99-103">Ak chcete povoliť rozšírenú ochranu pred hrozbami, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="90b99-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="90b99-104">Prejdite na konto [https://protection.office.com](https://protection.office.com) globálneho správcu alebo správcu zabezpečenia a prihláste sa pomocou konta správcu zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="90b99-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="90b99-105">Na ľavej navigačnej table v časti **Správa hrozieb**vyberte položku **Policy** \> **Prílohy bezpečné pre poistky**.</span><span class="sxs-lookup"><span data-stu-id="90b99-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="90b99-106">Vyberte položku **Zapnúť atp pre SharePoint, OneDrive a Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="90b99-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="90b99-107">[Vytvorte politiku upozornenia](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) na aktivitu na prijímanie upozornení, keď zistíme škodlivé súbory.</span><span class="sxs-lookup"><span data-stu-id="90b99-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="90b99-108">Úplné pokyny nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="90b99-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="90b99-109">**Poznámka:** Atp neprehľadá každý súbor v SharePointe Online, OneDrive for Business alebo Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="90b99-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="90b99-110">Súbory sa asynchrónne kontrolujú procesom, ktorý používa aktivitu zdieľania, aktivitu hosťa a signály hrozieb na identifikáciu škodlivých súborov.</span><span class="sxs-lookup"><span data-stu-id="90b99-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="90b99-111">Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="90b99-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
