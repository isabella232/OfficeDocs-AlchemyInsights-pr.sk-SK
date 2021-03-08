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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525441"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii

Vykonajte nasledujúce kroky:

1. Ak nie ste globálnym správcom, môžete vyhľadávať správy, ktoré je potrebné pridať do **skupiny rolí správcu eDiscovery** alebo na **rolu správy vyhľadávania súladu**. Ak chcete odstrániť správy, budete sa musieť zapojiť do **skupiny rolí Správa organizácie** alebo do **roly riadenia vyhľadávania a čistenia**. Povolenia pre tieto roly sa priraďujú v [Centre zabezpečenia & compliance.](https://protection.office.com)
2. Ak chcete nájsť správu, ktorú chcete odstrániť, [vytvorte vyhľadávanie obsahu](https://docs.microsoft.com/office365/securitycompliance/content-search) .
3. [Pripojte sa k zabezpečeniu & prostredie centrum dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Ak používate MFA, prečítajte si tieto pokyny: [pripojenie k zabezpečeniu & centrum dodržiavania súladu v prostredí s použitím viacnásobného overovania](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Odstránenie správy: `New-ComplianceSearchAction` Ak chcete správu odstrániť, spustite rutinu typu cmdlet. Odstránené správy sa presunú do priečinka s využiteľnými položkami používateľa. Príkaz príklad nájdete v časti [Krok 3: odstránenie správy.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
