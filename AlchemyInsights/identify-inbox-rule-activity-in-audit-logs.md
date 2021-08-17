---
title: Identifikácia aktivity pravidla doručenej pošty v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2bddd267abacabcd04b54271ade8ecf7b69fab914bcb8c103c806c31a388d2f5
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891310"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifikácia aktivity pravidla doručenej pošty v denníkoch auditu

Pomocou vyhľadávania denníka auditu v vyhľadávaciemu Centrum dodržiavania súladu pre Microsoft 365 na zobrazenie udalostí pravidla pre doručenú poštu (vytvorenie, úprava a odstránenie pravidiel pre doručenú poštu).

1. Vykonajte niektorý z týchto krokov:
   - V Centrum dodržiavania súladu pre Microsoft 365 prejdite <https://compliance.microsoft.com> na položku  \> **Audit riešenia.** Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portáli Microsoft 365 Defender prejdite <https://security.microsoft.com> na položku **Audit**. Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://security.microsoft.com/auditlogsearch> .

2. Na **karte Hľadať** na stránke **Audit** nakonfigurujte tieto nastavenia:
   - **Rozsah dátumu a času:** Vyberte rozsah dátumu a času v **poliach Začiatok** **a** Koniec.
   - **Aktivity:** Vyberte jednu alebo viac z nasledujúcich hodnôt:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Aktualizácia pravidiel pre doručenú poštu Outlook klienta**

3. Po dokončení kliknite na tlačidlo **Hľadať**. Aktivity sa zobrazia na novej **stránke Auditovanie.**

4. Výberom aktivity vo výsledkoch otvorte výlet podrobností. V poli Parametre sa zobrazujú informácie o nastaveniach pravidla **pre doručenú** poštu.

Ďalšie informácie nájdete v téme [Určenie, či používateľ vytvoril pravidlo pre doručenú poštu.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
