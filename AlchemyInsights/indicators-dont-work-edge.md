---
title: Indikátory nefungujú v prehliadači Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326276"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikátory nefungujú v prehliadači Edge

Po vytvorení indikátora sa jej neminie Aplikácia Edge (Smartscreen). Ďalšie informácie nájdete v téme [Vytváranie indikátorov IP adries a URL adries alebo domén.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>Krok 1: Uistite sa, že:

- Overte správnosť indikátora (žiadne preklepy v IP/URL, správna akcia, správne skupiny pre RBAC).
- Po vytvorení indikátora počkajte minimálne 2 hodiny, aby sa zohľadňovať prípadné časové oneskorenie.
- Skontrolujte, či sú systém (systém) v aplikácii Microsoft Defender pre koncový bod k dispozícii.
- Overte, či môžu systém (či) komunikovať s cloudom.
- Na testovacej lokalite overte, či je obrazovka SmartScreen povolená a [dostupná.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>Krok 2: Riešenie potenciálneho problému

- Uistite sa, že klient spĺňa požiadavky. Podrobnosti nájdete v téme [Vytváranie indikátorov IP adries a URL adries alebo domén.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Uistite sa, že používate najnovšiu verziu prehliadača Edge. Ak chcete zistiť najnovšiu verziu, pozrite si [časť Zistite, ktorú verziu Microsoft Edge máte.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Reštartujte prehliadač Edge.
- Prejdite na lokalitu, pre ktorú máte nastavenie indikátora. Ak sa lokalita nezobrazuje podľa očakávania, pokračujte krokom 3. 

## <a name="step-3-collect-data"></a>Krok 3: Zhromažďovanie údajov

- Zhromažďovanie **diagnostických údajov MDEClientAnalyzer.** Pokyny nájdete v téme [Problémy s onboardingami v aplikácii Microsoft Defender pre koncový bod.](issues-with-onboarding-machines.md)
- Ak ste si dobre nainštalovali a zhromažďovali sledovanie Fiddler, pozrite si [časť Telerik Fiddler.](http://www.telerik.com/fiddler)
- Ak uprednostňujete pokyny od podpory spoločnosti Microsoft, výberom ikony podpory nižšie otvorte prípad podpory.
