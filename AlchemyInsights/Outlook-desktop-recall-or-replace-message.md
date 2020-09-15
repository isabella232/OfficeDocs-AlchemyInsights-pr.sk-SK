---
title: Stiahnutie alebo nahradenie e-mailovej správy v Outlooku v počítači
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664005"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Odvolanie alebo nahradenie e-mailovej správy v Outlooku

- Ako správca môžete **odvolať správy v mene používateľov, ktorí používajú prostredie PowerShell**. Správy nemožno odvolať z centra spravovania.
- Môžete **vyvolať iba správy, ktoré sa odosielajú ľuďom vo vašej organizácii**. Ak bola správa odoslaná na adresu služby Gmail, môžete ju napríklad vyvolať.
- **Správy odoslané z outlooku 2016 v PC môžete vyvolať len**. Ak používateľ odošle správu pomocou Outlooku pre Mac alebo Outlooku na webe, nemôžete ju vyvolať.

Odvolanie alebo nahradenie e-mailovej správy:

1. Na table priečinok v ľavej časti okna Outlooku vyberte priečinok Odoslaná pošta.
1. Dvojitým kliknutím otvorte správu, ktorú chcete vyvolať.
1. Vyberte kartu **Správa** a potom vyberte položku **akcie**  >  **odvolať túto správu**.
1. Vyberte položku **Odstrániť neprečítané kópie tejto správy** alebo **Odstrániť neprečítané kópie a nahradiť ich novou správou**a potom vyberte **tlačidlo OK**.
1. Ak odosielate náhradnú správu, Vytvorte správu a potom vyberte položku **Odoslať**.
1. Úspech alebo neúspech odvolania správy závisí od nastavení príjemcu v Outlooku. Postup na kontrolu odvolania nájdete v [tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Vyhľadanie a odstránenie e-mailových správ vo vašej organizácii

- Ak nie ste globálnym správcom, konto sa musí pridať do roly správcu eDiscovery alebo na rolu správy vyhľadávania súladu, aby ste mohli vyhľadávať správy. Ak chcete odstrániť správy, budete sa musieť zapojiť do skupiny rolí Správa organizácie alebo do roly riadenia vyhľadávania a čistenia. Povolenia pre tieto roly sa priraďujú v [Centre zabezpečenia a dodržiavania súladu](https://go.microsoft.com/fwlink/?linkid=2083731).
- Ak chcete nájsť správu, ktorú chcete odstrániť, [vytvorte vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) .
- [Pripojenie k centru PowerShell zabezpečenia a dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ak používate viacnásobné overovanie, pozrite si tému [pripojenie k PowerShell v centre zabezpečenia a dodržiavania súladu so službou Microsoft 365 s použitím viacnásobného overovania](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).