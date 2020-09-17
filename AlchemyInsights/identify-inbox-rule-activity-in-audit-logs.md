---
title: Určenie aktivity pravidla pre doručenú poštu v denníkoch auditu
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779066"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Určenie aktivity pravidla pre doručenú poštu v denníkoch auditu

Pomocou vyhľadávania denníkov auditu v centre zabezpečenia dodržiavania súladu služieb Microsoft 365 & môžete zobraziť udalosti pravidla pre doručenú poštu (vytváranie, úprava a odstraňovanie pravidiel pre doručenú poštu).

1. Prihláste sa do [Centra zabezpečenia dodržiavania súladu so službou Microsoft 365 Security &](https://protection.office.com/).

2. Prejdite na stránku **Search**  >  **vyhľadávania denníka auditu** vyhľadávania.

3. V poliach **Počiatočný** dátum a **Koncový dátum** vyberte rozsah dátumov.

4. V časti **aktivity poštovej schránky servera Exchange**overte, či je pole **aktivity** nastavené na možnosť **New-InboxRule vytvoriť alebo upraviť alebo zapnúť/vypnúť pravidlo pre doručenú poštu**.

5. Kliknite na položku **Hľadať**.

Vo výsledkoch vyberte záznam auditu. V rozbaľovacom zozname Podrobnosti kliknite na položku **Ďalšie informácie**. V poli **parametre** sa zobrazí informácia o nastavení pravidiel pre doručenú poštu.

Ďalšie informácie nájdete v téme [určenie, či používateľ vytvoril pravidlo pre doručenú poštu](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) .
