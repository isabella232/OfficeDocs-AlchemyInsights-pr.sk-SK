---
title: Používanie DLP v pravidlách prenosu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915293"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="59b50-102">Používanie DLP v pravidlách prenosu</span><span class="sxs-lookup"><span data-stu-id="59b50-102">Using DLP in transport rules</span></span>

<span data-ttu-id="59b50-103">Ak chcete integrovať ochranu pred únikom údajov (DLP) do existujúceho prenosu, použite podmienku **Ak správa obsahuje... Citlivé informácie** v nastavení pravidla prenosu.</span><span class="sxs-lookup"><span data-stu-id="59b50-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="59b50-104">**Ďalšie podrobnosti nájdete v témach:**</span><span class="sxs-lookup"><span data-stu-id="59b50-104">**For more details, see:**</span></span>

- <span data-ttu-id="59b50-105">Integrované typy citlivých informácií DLP v pravidlách prenosu: [Integrácia pravidiel pre citlivé informácie](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="59b50-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="59b50-106">Môžete tiež otestovať pravidlo pomocou testu politiky alebo bez neho pomocou testovacieho režimu na pravidle.</span><span class="sxs-lookup"><span data-stu-id="59b50-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="59b50-107">Pravidlo otestujte najskôr 30 minút po jeho vytvorení.</span><span class="sxs-lookup"><span data-stu-id="59b50-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="59b50-108">Pozrite si tému [Testovanie toku pošty/pravidiel prenosu](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="59b50-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="59b50-109">**Poznámka**: Ak sa pokúšate implementovať novú politiku DLP s pravidlami prenosu v EAC, použite namiesto toho [politiky DLP v centre zabezpečenia a dodržiavania súladu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="59b50-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
