---
title: Konfigurácia služby synchronizácie MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482898"
---
# <a name="configure-mim-sync-service"></a>Konfigurácia služby synchronizácie MIM

Služba synchronizácie Microsoft Identity Manager (MIM) je súčasťou MIM. Ide o centralizovanú lokálnu službu, ktorá ukladá a integruje informácie o organizáciách s viacerými lokálnymi adresármi a databázami. Problém s synchronizáciou MIM môžete vyriešiť v prípade, že problém bol vyriešený v poslednej aktualizácii na MIM alebo je jedným z ďalších problémov uvedených v časti nižšie.

**Odporúčané kroky**

1. Uistite sa, že používate nedávnu aktualizáciu synchronizácie MIM a skontrolujte poznámky k [vydaniu synchronizácie Mim](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) a zistite, či sa problém vyriešil v aktualizácii.
2. Ak sa vyskytol problém s doplnkom generických protokolov LDAP, Generic SQL, Lotus Domino alebo Web Services, skontrolujte, či používate nedávnu aktualizáciu [všeobecných spojníc](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Ak sa synchronizácia MIM spustí s chybou, prečítajte si tabuľku [chybových kódov spustiť](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) , aby ste určili možné príčiny.
4. Ak sa spustiť zastaví s **rozšírením – DLL – výnimka**, kliknite na tieto slová a otvorte okno **Vlastnosti objektu spojnice** a kliknite na položku **sledovanie zásobníka..** . a zobrazia sa ďalšie informácie o príčine, ako je to popísané v téme [rozšírenie – dll – výnimka](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Ak sa pri synchronizácii hesla v denníku udalostí počas synchronizácie hesiel **zobrazí chybové** hlásenie o tom, že v príručke na riešenie problémov s [vyhlásením služby PCNS sa 6025 zobrazí](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)chyba 6025.
6. Ak je úplná synchronizácia s agentom správy služby FIM pomalá, skontrolujte nastavenie **automatického rastu** pre tempdb, ako je popísané v časti [Riešenie problémov s pomalým alebo zavesením úplnej synchronizácie](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Ak sa vyskytne chyba zastaveného servera s neúspešným vytvorením-cez-Web-Services pomocou agenta správy služby FIM, prečítajte si tému [Technická podpora – informácie: zlyhanie – vytvorenie – cez – web – služby](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) na prehľad príčin.

