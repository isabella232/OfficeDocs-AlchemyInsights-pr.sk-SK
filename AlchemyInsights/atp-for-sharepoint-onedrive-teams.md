---
title: ATP pre SharePoint, OneDrive a Microsoft teams
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715576"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="f84eb-102">ATP pre SharePoint, OneDrive a Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="f84eb-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="f84eb-103">Ak chcete povoliť rozšírenú ochranu pred hrozbami, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="f84eb-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="f84eb-104">Prejdite na [https://protection.office.com](https://protection.office.com) globálneho správcu alebo konto správcu zabezpečenia a prihláste sa.</span><span class="sxs-lookup"><span data-stu-id="f84eb-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="f84eb-105">Na ľavej navigačnej table v časti **Správa hrozieb**vyberte položku **Policy** \> **bezpečnostné prílohy**politiky.</span><span class="sxs-lookup"><span data-stu-id="f84eb-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="f84eb-106">Vyberte položku **Zapnúť ATP pre SharePoint, OneDrive a Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="f84eb-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="f84eb-107">Pri zisťovaní škodlivých súborov [vytvorte politiku upozornenia o aktivite](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) na prijímanie oznámení.</span><span class="sxs-lookup"><span data-stu-id="f84eb-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="f84eb-108">Podrobné pokyny nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="f84eb-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="f84eb-109">**Poznámka**: zámerom je, že ATP neskenuje každý jeden súbor v SharePointe Online, OneDrive for Business alebo v aplikácii Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="f84eb-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="f84eb-110">Súbory sa kontrolujú asynchrónne procesom, ktorý používa aktivitu zdieľania, aktivitu hostí a signály hrozby na identifikáciu škodlivých súborov.</span><span class="sxs-lookup"><span data-stu-id="f84eb-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="f84eb-111">Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="f84eb-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
