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
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742770"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Vyvolanie alebo nahradenie e-mailovej správy v Microsoft 365

- Môžete **pripomenúť iba správy odoslané ľuďom vo vašej organizácii**. Ak bola správa odoslaná na adresu služby Gmail, nemôžete ju napríklad pripomenúť.
- Môžete si **len pripomenúť správy odoslané z programu Outlook 2016 pre PC**. Ak používateľ odošle správu pomocou programu Outlook for Mac alebo Outlook na webe, nemôžete pripomenúť.
- Ak ste správcom, môžete si **pripomenúť správy v mene používateľov pomocou prostredia PowerShell**. Správy z centra spravovania nemožno vyvolať. Prejdite na "vyhľadať a odstrániť e-mailové správy v organizácii" pre viac informácií.

**Vyvolanie alebo nahradenie e-mailovej správy, ktorú ste odoslali**

1. Na table priečinkov v ľavej časti okna programu Outlook vyberte priečinok Odoslaná pošta.
2. Otvorte správu, ktorú chcete pripomenúť. Ak chcete otvoriť správu, musíte dvakrát kliknúť. Výber správy tak, že sa zobrazí na table na čítanie, vám nedovolí pripomenúť správu.
3. Na karte Správa vyberte položku **akcie** > **vyvolanie tejto správy**.
4. Vyberte položku **Odstrániť neprečítané kópie tejto správy** alebo **odstráňte neprečítané kópie a nahraďte ju novou správou a**potom kliknite na **tlačidlo OK**.
5. Ak odosielate náhradnú správu, napíšte správu a potom vyberte položku **Odoslať**.
6. Úspech alebo neúspech odvolanie správy závisí od nastavenia príjemcov v programe Outlook.

Ďalšie informácie vrátane informácií o tom, ako skontrolovať odvolanie, nájdete v časti [vyvolanie alebo nahradenie e-mailovej správy, ktorú ste odoslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Vyhľadávanie a odstraňovanie e-mailových správ vo vašej organizácii*** Ak chcete vyhľadávať a odstraňovať e-mailové správy vo vašej organizácii, je to najjednoduchšie, ak ste globálny správca. Ak nie ste globálny správca, konto sa musí pridať do skupiny rolí eDiscovery Manager alebo do roly správy vyhľadávania súladu. Ak chcete odstrániť správy, musíte sa pripojiť k skupine rolí Správa organizácie alebo k úlohe správy vyhľadávania a čistenia. Povolenia pre tieto roly sú priradené v [Centre zabezpečenia & súladu](https://protection.office.com/).

1. [Vytvorte hľadanie obsahu](https://docs.microsoft.com/office365/securitycompliance/content-search) a vyhľadajte správu, ktorá sa má odstrániť.
2. [Pripojenie k zabezpečeniu & centrum PowerShell súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Ak používate MFA, pozrite si [pripojiť k Microsoft 365 zabezpečenia & Compliance Center PowerShell pomocou viacnásobné overovanie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
