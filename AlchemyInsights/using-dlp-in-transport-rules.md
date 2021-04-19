---
title: Používanie DLP v pravidlách prenosu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827231"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="f54f7-102">Používanie DLP v pravidlách prenosu</span><span class="sxs-lookup"><span data-stu-id="f54f7-102">Using DLP in transport rules</span></span>

<span data-ttu-id="f54f7-103">Ak chcete integrovať ochranu pred únikom údajov (DLP) do existujúceho prenosu, použite podmienku **Ak správa obsahuje... Citlivé informácie** v nastavení pravidla prenosu.</span><span class="sxs-lookup"><span data-stu-id="f54f7-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="f54f7-104">**Ďalšie podrobnosti nájdete v témach:**</span><span class="sxs-lookup"><span data-stu-id="f54f7-104">**For more details, see:**</span></span>

- <span data-ttu-id="f54f7-105">Integrované typy citlivých informácií DLP v pravidlách prenosu: [Integrácia pravidiel pre citlivé informácie](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="f54f7-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="f54f7-106">Môžete tiež otestovať pravidlo pomocou testu politiky alebo bez neho pomocou testovacieho režimu na pravidle.</span><span class="sxs-lookup"><span data-stu-id="f54f7-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="f54f7-107">Pravidlo otestujte najskôr 30 minút po jeho vytvorení.</span><span class="sxs-lookup"><span data-stu-id="f54f7-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="f54f7-108">Pozrite si tému [Testovanie toku pošty/pravidiel prenosu](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="f54f7-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="f54f7-109">**Poznámka**: Ak sa pokúšate implementovať novú politiku DLP s pravidlami prenosu v EAC, použite namiesto toho [politiky DLP v centre zabezpečenia a dodržiavania súladu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f54f7-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
