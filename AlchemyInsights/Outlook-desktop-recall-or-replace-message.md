---
title: Stiahnutie alebo nahradenie e-mailovej správy v aplikácii Outlook Desktop
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502334"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Vyvolanie alebo nahradenie e-mailovej správy programu Outlook

- Ako správca si môžete **vyvolať správy v mene používateľov pomocou prostredia PowerShell**. Správy nemôžete vyvolať z Centra spravovania.
- Môžete **si spomenúť len na správy odoslané osobám vo vašej organizácii.** Ak bola napríklad správa odoslaná na adresu Gmail, nemôžete si ju spomenúť.
- Správy **odoslané z Outlooku 2016**v počítači môžete vyvolať iba . Ak používateľ odošle správu pomocou Outlooku for Mac alebo Outlooku na webe, nemôžete si ju spomenúť.

Stiahnutie alebo nahradenie e-mailovej správy:

1. Na table priečinkov v ľavej časti okna programu Outlook vyberte priečinok Odoslaná pošta.
1. Dvojitým kliknutím otvorte správu, ktorú si chcete vyvolať.
1. Vyberte kartu **Správa** a potom vyberte položku **Akcie**  >  **Vyvolať túto správu**.
1. Vyberte položku **Odstrániť neprečítané kópie tejto správy** alebo Odstrániť **neprečítané kópie a nahradiť novou správou**a potom vyberte **tlačidlo OK**.
1. Ak odosielate náhradnú správu, napíšte správu a potom vyberte položku **Odoslať**.
1. Úspech alebo neúspech odvolania správy závisí od nastavení príjemcu v programe Outlook. Postup na kontrolu stiahnutia nájdete v [tomto článku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Vyhľadávanie a odstraňovanie e-mailových správ v organizácii

- Ak nie ste globálnym správcom, váš účet musí byť pridaný do roly správcu elektronického vyhľadávania alebo roly správy vyhľadávania súladu, aby ste mohli vyhľadávať správy. Ak chcete odstrániť správy, musíte sa pripojiť k skupine rolí Správa organizácie alebo rolu správy Vyhľadávania a vymazania. Povolenia pre tieto roly sú priradené v [centre zabezpečenia a súladu](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Vytvorte vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/content-search) a vyhľadajte správu, ktorá sa má odstrániť.
- [Pripojte sa k PowerShell centra zabezpečenia a dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ak používate viacnásobné overovanie, pozrite si tému [Pripojenie k prostrediu PowerShell centra zabezpečenia a dodržiavania súladu](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)pomocou viacnásobného overovania .