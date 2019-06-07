---
title: ATP pre SharePoint a OneDrive Microsoft tímy
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765388"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="d6de8-102">ATP pre SharePoint a OneDrive Microsoft tímy</span><span class="sxs-lookup"><span data-stu-id="d6de8-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="d6de8-103">Postupujte nasledovne umožniť rozšírenú ochranu:</span><span class="sxs-lookup"><span data-stu-id="d6de8-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="d6de8-104">Prejsť na [https://protection.office.com](https://protection.office.com) a prihláste sa pomocou globálny správca alebo správca konto zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="d6de8-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="d6de8-105">Na ľavej navigačnej table pod **Threat management**vyberte **politika** \> **Bezpečnými prílohami**.</span><span class="sxs-lookup"><span data-stu-id="d6de8-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="d6de8-106">Vyberte **Zapnúť ATP pre SharePoint, OneDrive, a tímy Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="d6de8-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="d6de8-107">[Vytvorenie aktivity alert politiky](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) dostávať upozornenia, keď sme odhaliť škodlivé súbory.</span><span class="sxs-lookup"><span data-stu-id="d6de8-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="d6de8-108">Kompletné pokyny nájdete v časti tejto [témy](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="d6de8-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="d6de8-109">**Poznámka**: predvolene ATP neprehľadáva každý súbor v službe SharePoint Online, OneDrive for Business alebo Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d6de8-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="d6de8-110">Súbory sú načítané asynchrónne proces, ktorý využíva zdieľanie činností, hodnotenie a hrozba signály na identifikáciu škodlivého súborov.</span><span class="sxs-lookup"><span data-stu-id="d6de8-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="d6de8-111">Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="d6de8-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
