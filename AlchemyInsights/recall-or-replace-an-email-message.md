---
title: Vyvolanie alebo nahradenie e-mailovej správy
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509471"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Vyvolanie alebo nahradenie e-mailovej správy v službe Microsoft 365

- Môžete **si spomenúť len na správy odoslané osobám vo vašej organizácii.** Ak bola napríklad správa odoslaná na adresu Gmail, nemôžete si ju spomenúť.
- Môžete **si spomenúť len na správy odoslané z Outlooku 2016 pre počítač**. Ak používateľ odošle správu pomocou Outlooku for Mac alebo Outlooku na webe, nemôžete si ju spomenúť.
- Ak ste správcom, správy môžete **vyvolať v mene používateľov pomocou prostredia PowerShell**. Správy nemôžete vyvolať z Centra spravovania. Ďalšie informácie získate nadol na položku Vyhľadať a odstrániť e-mailové správy vo vašej organizácii.

**Vyvolanie alebo nahradenie odoslanej e-mailovej správy**

1. Na table priečinkov v ľavej časti okna programu Outlook vyberte priečinok Odoslaná pošta.
2. Otvorte správu, ktorú si chcete odvolať. Ak chcete správu otvoriť, musíte dvakrát kliknúť. Výber správy tak, aby sa zobrazila na table na čítanie, vám neumožní vyvolať správu.
3. Na karte Správa vyberte položku **Akcie**  >  **Vyvolať túto správu**.
4. Vyberte **položku Odstrániť neprečítané kópie tejto správy** alebo Odstrániť **neprečítané kópie a nahradiť novou správou a**potom vyberte tlačidlo **OK**.
5. Ak odosielate náhradnú správu, napíšte správu a vyberte položku **Odoslať**.
6. Úspech alebo neúspech odvolania správy závisí od nastavení príjemcov v programe Outlook.

Ďalšie informácie vrátane kontroly stiahnutia z trhu nájdete v téme [Vyvolanie alebo nahradenie odoslanej e-mailovej správy](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Vyhľadávanie a odstraňovanie e-mailových správ v organizácii*** Ak chcete vyhľadávať a odstraňovať e-mailové správy vo vašej organizácii, je najjednoduchšie, ak ste globálnysprávca. Ak nie ste globálnym správcom, váš účet musí byť pridaný do skupiny rolí eDiscovery Manager alebo do roly správy vyhľadávania súladu. Ak chcete odstrániť správy, musíte sa pripojiť k skupine rolí Správa organizácie alebo rolu správy Vyhľadávania a vymazania. Povolenia pre tieto roly sú priradené v [centre zabezpečenia & súladu](https://protection.office.com/).

1. [Vytvorte vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) a vyhľadajte správu, ktorá sa má odstrániť.
2. [Pripojte sa k službe PowerShell centra zabezpečenia & Centra zabezpečenia](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Ak používate mfa, pozrite si tému [Pripojenie k službe Microsoft 365 & prostredia PowerShell centra súladu pomocou viacnásobného overovania](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
