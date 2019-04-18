---
title: Doručená pošta pravidlo aktivitu v denníkoch auditu určiť
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909542"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="1b1e2-102">Doručená pošta pravidlo aktivitu v denníkoch auditu určiť</span><span class="sxs-lookup"><span data-stu-id="1b1e2-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="1b1e2-103">Vyhľadávanie denník auditu v & zabezpečenia súladu centra môžete zobraziť priečinok Doručená pošta pravidlo akcie (vytváranie, úpravu a odstránenie pravidiel pre doručenú poštu).</span><span class="sxs-lookup"><span data-stu-id="1b1e2-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="1b1e2-104">Prihláste sa do [Centrum Office 365 zabezpečenia & súlad](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="1b1e2-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="1b1e2-105">Kliknite na položku **vyhľadávanie a vyšetrovanie** a vyberte **Vyhľadávanie denník auditu**.</span><span class="sxs-lookup"><span data-stu-id="1b1e2-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="1b1e2-106">Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Koncový dátum** .</span><span class="sxs-lookup"><span data-stu-id="1b1e2-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="1b1e2-107">Časti **Exchange schránky aktivít**, overenie **činnosti** pole nastavené na **New-InboxRule vytvoriť/upraviť/zapnúť/vypnúť pravidlo pre doručenú poštu**.</span><span class="sxs-lookup"><span data-stu-id="1b1e2-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="1b1e2-108">Kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="1b1e2-108">Click **Search**.</span></span>

<span data-ttu-id="1b1e2-109">V zozname výsledkov vyberte auditný záznam.</span><span class="sxs-lookup"><span data-stu-id="1b1e2-109">In the results, select an audit record.</span></span> <span data-ttu-id="1b1e2-110">V rozbaľovacie tlačidlo Podrobnosti, kliknite na **Viac informácií**.</span><span class="sxs-lookup"><span data-stu-id="1b1e2-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="1b1e2-111">Zobrazia sa informácie o nastavenie pravidla priečinka doručenej pošty v poli **parametre** .</span><span class="sxs-lookup"><span data-stu-id="1b1e2-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="1b1e2-112">Pre viac informácie, pozri [určenie ak užívateľ vytvoril pravidlo pre doručenú poštu](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="1b1e2-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
