---
title: Defender Endpoint check sensor status
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676337"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender Endpoint check sensor status

Dlaždica **Zariadenia s problémami senzora** sa nachádza na tabuli Operácie zabezpečenia. Táto dlaždica poskytuje informácie o schopnosti jednotlivých zariadení poskytovať údaje senzora a komunikovať so službu Defender pre koncový bod. V tejto matici sa nachádza hlásenie, koľko zariadení vyžaduje pozornosť, a pomáha identifikovať problematické zariadenia a prijať opatrenia na odstránenie známych problémov.

Dva indikátory stavu na dlaždici poskytujú informácie o počte zariadení, ktoré sa službe nesprávne nahlasujú:

- **Nesprávne nakonfigurované** Zariadenia, ktoré môžu čiastočne vykazovať údaje senzora do služby Defender pre koncové body a môžu mať chyby konfigurácie, ktoré je potrebné opraviť.
- **Neaktívne** Zariadenia, ktoré zastavili vykazovanie do služby Defender for Endpoint na viac ako sedem dní v priebehu minulého mesiaca.

Po kliknutí na niektorú zo skupín sa nasmeruje na zoznam Zariadenia filtrovaný podľa vašich možností. V zozname Zariadenia môžete zoznam stavov filtrovať podľa tohto stavu:

- **Aktívne** Zariadenia, ktoré aktívne hlásia službu Defender pre koncový bod.
- **Nesprávne nakonfigurované** Zariadenia, ktoré môžu čiastočne vykazovať údaje senzora do služby Defender pre koncový bod, ale majú chyby konfigurácie, ktoré je potrebné opraviť. Nesprávne nakonfigurované zariadenia môžu mať jeden alebo kombináciu nasledujúcich problémov:

    - Žiadne údaje senzora – zariadenia prestali odosielať údaje senzora. Zo zariadenia možno spustiť obmedzené upozornenia.
    - Komunikácia s poruchou – možnosť komunikácie so zariadením je s poruchou. Odosielanie súborov na podrobnú analýzu, blokovanie súborov, izolovanie zariadení od siete a ďalšie akcie, ktoré vyžadujú komunikáciu so zariadením, nemusia fungovať.
- **Neaktívne** Zariadenia, ktoré prestali vykazovať službu Defender pre koncový bod.

Celý zoznam vo formáte CSV môžete stiahnuť pomocou funkcie Exportovať.

Ďalšie informácie nájdete v téme [Kontrola stavu senzora v aplikácii Microsoft Defender pre koncový bod.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Ďalšie informácie o tom, čo spôsobilo neaktívne alebo nesprávne nakonfigurované zariadenie, nájdete v téme Oprava nevhodných senzorov v [aplikácii Microsoft Defender pre koncový bod.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
