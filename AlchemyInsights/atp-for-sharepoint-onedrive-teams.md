---
title: ATP pre SharePoint, OneDrive a Microsoft teams
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
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712473"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="715fc-102">ATP pre SharePoint, OneDrive a Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="715fc-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="715fc-103">Ak chcete povoliť rozšírenú ochranu pred hrozbami, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="715fc-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="715fc-104">Prejdite na [https://protection.office.com](https://protection.office.com) a prihláste sa pomocou globálneho správcu alebo konta správcu zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="715fc-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="715fc-105">Na ľavej navigačnej table v časti **Správa hrozieb**vyberte položku **Policy** \> **bezpečné prílohy**politiky.</span><span class="sxs-lookup"><span data-stu-id="715fc-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="715fc-106">Vyberte možnosť **Zapnúť ATP pre SharePoint, OneDrive a Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="715fc-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="715fc-107">[Vytvorenie politiky výstrahy aktivity](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) na prijímanie upozornení pri detekcii škodlivých súborov.</span><span class="sxs-lookup"><span data-stu-id="715fc-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="715fc-108">Úplné pokyny nájdete v tejto [téme](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="715fc-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="715fc-109">**Poznámka**: podľa návrhu, ATP neskenuje každý jednotlivý súbor SharePoint Online, OneDrive pre podniky alebo Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="715fc-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="715fc-110">Súbory sú naskenované asynchrónne procesom, ktorý používa zdieľanie aktivity, hodnotenie aktivity a hrozby signály identifikovať škodlivé súbory.</span><span class="sxs-lookup"><span data-stu-id="715fc-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="715fc-111">Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="715fc-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
