---
title: Určenie aktivity pravidla pre doručenú poštu v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779066"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="2af23-102">Určenie aktivity pravidla pre doručenú poštu v denníkoch auditu</span><span class="sxs-lookup"><span data-stu-id="2af23-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="2af23-103">Pomocou vyhľadávania denníkov auditu v centre zabezpečenia dodržiavania súladu služieb Microsoft 365 & môžete zobraziť udalosti pravidla pre doručenú poštu (vytváranie, úprava a odstraňovanie pravidiel pre doručenú poštu).</span><span class="sxs-lookup"><span data-stu-id="2af23-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="2af23-104">Prihláste sa do [Centra zabezpečenia dodržiavania súladu so službou Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="2af23-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="2af23-105">Prejdite na stránku **Search**  >  **vyhľadávania denníka auditu** vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="2af23-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="2af23-106">V poliach **Počiatočný** dátum a **Koncový dátum** vyberte rozsah dátumov.</span><span class="sxs-lookup"><span data-stu-id="2af23-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="2af23-107">V časti **aktivity poštovej schránky servera Exchange**overte, či je pole **aktivity** nastavené na možnosť **New-InboxRule vytvoriť alebo upraviť alebo zapnúť/vypnúť pravidlo pre doručenú poštu**.</span><span class="sxs-lookup"><span data-stu-id="2af23-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="2af23-108">Kliknite na položku **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="2af23-108">Click **Search**.</span></span>

<span data-ttu-id="2af23-109">Vo výsledkoch vyberte záznam auditu.</span><span class="sxs-lookup"><span data-stu-id="2af23-109">In the results, select an audit record.</span></span> <span data-ttu-id="2af23-110">V rozbaľovacom zozname Podrobnosti kliknite na položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="2af23-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2af23-111">V poli **parametre** sa zobrazí informácia o nastavení pravidiel pre doručenú poštu.</span><span class="sxs-lookup"><span data-stu-id="2af23-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="2af23-112">Ďalšie informácie nájdete v téme [určenie, či používateľ vytvoril pravidlo pre doručenú poštu](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) .</span><span class="sxs-lookup"><span data-stu-id="2af23-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
