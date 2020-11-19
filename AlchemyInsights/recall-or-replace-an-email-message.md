---
title: Odvolanie alebo nahradenie e-mailovej správy
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353521"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Odvolanie alebo nahradenie e-mailovej správy v programe Microsoft 365

- Môžete **vyvolať iba správy, ktoré sa odosielajú ľuďom vo vašej organizácii**. Ak ste napríklad správu odoslali na adresu služby Gmail, nemôžete ju vyvolať.
- Odvolať sa môžete **len na správy odoslané z Outlooku pre PC**. Ak používateľ odošle správu pomocou Outlooku pre Mac alebo Outlooku na webe, nemôžete ju vyvolať.
- Ako správca nájomníkov môžete v **mene používateľov odvolať správy pomocou prostredia PowerShell** (Ďalšie informácie nájdete v téme: [Vyhľadanie a odstránenie e-mailových správ](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Správy nemožno odvolať z centra spravovania. Ďalšie informácie nájdete v časti Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii.

**Odvolanie alebo nahradenie e-mailovej správy, ktorú ste odoslali**

1. Na table priečinok v ľavej časti okna Outlooku vyberte priečinok Odoslaná pošta.
2. Otvorte správu, ktorú chcete odvolať. Ak chcete správu otvoriť, musíte dvakrát kliknúť. Ak vyberiete správu tak, aby sa zobrazila na table na čítanie, nebudete môcť správu odvolať.
3. Na karte Správa vyberte položku **akcie**  >  **odvolať túto správu**.
4. Vyberte položku **Odstrániť neprečítané kópie tejto správy** alebo **Odstrániť neprečítané kópie a nahradiť ich novou správou a** potom vyberte **tlačidlo OK**.
5. Ak odosielate náhradnú správu, Vytvorte správu a potom vyberte položku **Odoslať**.
6. Úspešné alebo neúspešné odvolanie správy závisí od nastavení príjemcov v Outlooku.

Ďalšie informácie vrátane informácií o tom, ako skontrolovať odvolanie, nájdete v téme [odvolanie alebo nahradenie e-mailovej správy, ktorú ste odoslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Ak chcete **_Vyhľadať a odstrániť e-mailové správy vo vašej organizácii_**, je to najjednoduchšie, ak ste globálnym správcom. Ak nie ste globálnym správcom, vaše konto sa musí pridať do skupiny rolí správcu eDiscovery alebo na rolu riadenia vyhľadávania súladu. Ak chcete odstrániť správy, budete sa musieť zapojiť do skupiny rolí Správa organizácie alebo do roly riadenia vyhľadávania a čistenia. Povolenia pre tieto roly sa priraďujú v [Centre zabezpečenia & Compliance](https://protection.office.com/).

1. Ak chcete nájsť správu, ktorú chcete odstrániť, [vytvorte vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) .
2. [Pripojte sa k zabezpečeniu & prostredie centrum dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Ak používate MFA (viacnásobné overovanie), pozrite si tému [pripojenie k službe Microsoft 365 Security & centrum dodržiavania súladu v prostredí s použitím viacnásobného overovania](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
