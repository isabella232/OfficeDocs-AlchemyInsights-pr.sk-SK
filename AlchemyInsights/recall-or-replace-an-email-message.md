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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024401"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Odvolanie alebo nahradenie e-mailovej správy vo Microsoft 365

- Odvolať môžete **len správy odoslané ľuďom vo vašej organizácii.** Ak bola napríklad správa odoslaná na adresu služby Gmail, nemôžete ju odvolať.
- Odvolať môžete **len správy odoslané z Outlook počítača.** Ak používateľ odošle správu pomocou Outlook pre Mac alebo Outlook na webe, nemôžete ju odvolať.
- Ako správca nájomníkov môžete odvolať správy v mene používateľov pomocou prostredia **PowerShell** (Ďalšie informácie nájdete v téme: Vyhľadanie a odstránenie [e-mailových správ).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- V Centre spravovania nie je možné odvolať správy. Ďalšie informácie nájdete v časti "Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii".

**Odvolanie alebo nahradenie odoslaných e-mailových správ**

1. Na table priečinka na ľavej strane okna Outlook vyberte priečinok Odoslaná pošta.
2. Otvorte správu, ktorú chcete odvolať. Správu musíte otvoriť dvojitým kliknutím. Výber správy tak, že sa zobrazí v table na čítanie, vám neuvolí odvolať správu.
3. Na karte Správa vyberte položku Akcie **odvolať**  >  **túto správu**.
4. Vyberte **položku Odstrániť neprečítané kópie tejto správy** alebo Odstrániť **neprečítané** kópie a nahradiť ich novou správou a potom vyberte tlačidlo **OK**.
5. Ak odosielate náhradnú správu, napíšte ju a potom vyberte položku **Odoslať**.
6. Úspech alebo neúspech odvolávania správy závisí od nastavení príjemcu v Outlook.

Ďalšie informácie vrátane kontroly odvolania nájdete v téme Odvolanie alebo nahradenie [odoslanej e-mailovej správy.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Ak chcete vyhľadať a odstrániť e-mailové správy*** v organizácii, najjednoduchšie je, ak ste globálnym správcom. Ak nie ste globálnym správcom, vaše konto je potrebné pridať do skupiny rolí eDiscovery Manager alebo do roly správy vyhľadávania súladu. Ak chcete odstrániť správy, musíte sa pripojiť k skupine rolí Správa organizácie alebo k role správy vyhľadávania a vymazania. Povolenia týchto rolí sú priradené v Centre [zabezpečenia & dodržiavania súladu.](https://protection.office.com/)

1. [Vytvorte vyhľadávanie obsahu a](https://docs.microsoft.com/microsoft-365/compliance/content-search) vyhľadajte správu na odstránenie.
2. [Pripojenie na centrum zabezpečenia & PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Ak používate VIACFAktorové overovanie, pozrite si Pripojenie Microsoft 365 zabezpečenia & PowerShell pomocou [viacfaktorového overovania.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
