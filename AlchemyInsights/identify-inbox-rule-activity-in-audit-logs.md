---
title: Identifikácia aktivity pravidla doručenej pošty v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716439"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="fd34a-102">Identifikácia aktivity pravidla doručenej pošty v denníkoch auditu</span><span class="sxs-lookup"><span data-stu-id="fd34a-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="fd34a-103">Vyhľadávanie denníka auditu môžete použiť v Microsoft 365 zabezpečenia & Compliance Center Zobraziť udalosti pravidlo pre doručenú poštu (vytváranie, upravovanie a odstraňovanie pravidiel pre doručenú poštu).</span><span class="sxs-lookup"><span data-stu-id="fd34a-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="fd34a-104">Prihláste sa do [Microsoft 365 Security & centrum súladu](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="fd34a-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="fd34a-105">Prejdite na stránku vyhľadávania**denníka auditu** **vyhľadávania** > .</span><span class="sxs-lookup"><span data-stu-id="fd34a-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="fd34a-106">Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Dátum ukončenia** .</span><span class="sxs-lookup"><span data-stu-id="fd34a-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="fd34a-107">V časti **aktivity poštovej schránky servera Exchange**, skontrolujte **aktivity** pole nastavená na **nové InboxRule vytvoriť/upraviť/Povoliť/zakázať Doručená pošta pravidlo**.</span><span class="sxs-lookup"><span data-stu-id="fd34a-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="fd34a-108">Kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="fd34a-108">Click **Search**.</span></span>

<span data-ttu-id="fd34a-109">Vo výsledkoch vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="fd34a-109">In the results, select an audit record.</span></span> <span data-ttu-id="fd34a-110">V rozbaľovacom zozname Podrobnosti kliknite na položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="fd34a-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="fd34a-111">Informácie o nastavení pravidiel pre doručenú poštu sa zobrazia v poli **parametre** .</span><span class="sxs-lookup"><span data-stu-id="fd34a-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="fd34a-112">Ďalšie informácie nájdete v téme [určenie, či používateľ vytvoril pravidlo pre doručenú poštu](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="fd34a-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
