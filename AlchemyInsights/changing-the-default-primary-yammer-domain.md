---
title: Zmena predvolenej domény Yammer
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
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818015"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Zmena predvolenej/primárnej domény Yammer

URL adresa Yammera obsahuje názov aktuálnej primárnej domény siete Yammer. Tento názov domény sa nemusí zhodovať s primárnymi názvami domén, ktoré sú nastavené v Office 365 alebo Azure AD. Správanie sa líši v závislosti od počtu vlastných domén pridaných do nájomníka a od toho, či sa Yammer nachádza v podporovanej konfigurácii (1 nájomník: 1 sieť alebo 1:1). K dispozícii je dokumentácia o [doménach Yammer a Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Najčastejším dôvodom zobrazovania nesprávnej domény je, že existuje viacero sietí Yammer a je potrebné ich zlúčiť. [Zlúčenie sietí do jednej](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) pomocou nástroja na migráciu sietí je dôležitým prvým krokom. Tento krok vykonajte ešte pred tým, než sa pokúsite nastaviť primárnu doménu.

**Žiadne vlastné domény**

Pre nových nájomníkov sa pre Yammer použije predvolená doména (napríklad fabrikam.onmicrosoft.com) z nájomníka. Primárna doména je nastavená na yammer.com/fabrikam.onmicrosoft.com.

**Jedna vlastná doména**

Yammer automaticky vyberie vlastnú doménu (napríklad fabrikam.com) z nájomníka ako primárnu doménu v Yammeri. Je nastavená na yammer.com/fabrikam.com. Túto zmenu vykoná služba synchronizácie domén a jej prejavenie môže trvať až 24 hodín.

**Viaceré vlastné domény**

Yammer môže mať primárnu doménu, ktorá sa líši od predvolenej domény nájomníka. Keďže existuje viacero vlastných domén, Yammer sa nepokúša uhádnuť tú správnu z tých, ktoré sú k dispozícii. Ak chcete zmeniť primárny názov domény na primárnu doménu podľa vlastného výberu, musíte otvoriť prípad podpory.

**Ďalšie informácie o riešení problémov**

V niektorých prípadoch sa môžu domény premiestňovať medzi nájomníkmi a služba synchronizácie domén sa nedokázala úspešne spustiť. Okrem nesprávnej primárnej domény sa môžu vyskytnúť problémy s prihlásením alebo iné chyby. Ak chcete vyriešiť tento problém, možno bude potrebné premiestniť domény do správnej siete s pomocou podpory spoločnosti Microsoft. Táto situácia vyžaduje priamu pomoc a jej riešenie môže chvíľu trvať, a to najmä v prípade, že máte veľmi dlhý zoznam názvov domén. Otvorte prípad podpory, čím získate pomoc pri riešení týchto typov problémov.

Pri práci so zástupcom oddelenia podpory skontroluje, či sa domény overujú v nájomníkovi, nad ktorým máte kontrolu. V prípade, že sa domény pridajú do vášho nájomníka, ale nie sú overené službou DNS, zástupca vám môže položiť ďalšie otázky na ich overenie. Ak chcete urýchliť proces, uistite sa, že domény sú overené službou DNS.
