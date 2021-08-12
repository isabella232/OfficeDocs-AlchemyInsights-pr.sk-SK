---
title: Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948898"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii

Vykonajte nasledujúce kroky:

1. Ak nie ste globálnym správcom, na vyhľadanie správ je potrebné, aby sa vaše konto pridalo do skupiny rolí **eDiscovery Manager** alebo rola správy **vyhľadávania súladu.** Ak chcete odstrániť správy, musíte sa pripojiť k skupine rolí Správa **organizácie** alebo k **role správy vyhľadávania a vymazania.** Povolenia týchto rolí sa priraďujú v [Centre zabezpečenia & dodržiavania súladu.](https://protection.office.com)
2. [Vytvorte vyhľadávanie obsahu a](https://docs.microsoft.com/office365/securitycompliance/content-search) vyhľadajte správu na odstránenie.
3. [Pripojenie na centrum zabezpečenia & PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Ak používate MFA, pozrite si tieto pokyny: Pripojenie zabezpečenia [& zabezpečenia pomocou viacfaktorového overovania](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Odstráňte hlásenie: ak chcete `New-ComplianceSearchAction` správu odstrániť, spustite rutinu typu cmdlet. Odstránené správy sa premiestnia do priečinka Obnoviteľné položky používateľa. Príklad príkazu nájdete v časti [Krok 3: Odstránenie správy.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
