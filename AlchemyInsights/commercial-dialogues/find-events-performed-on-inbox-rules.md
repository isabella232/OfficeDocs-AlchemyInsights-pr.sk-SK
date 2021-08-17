---
title: Vyhľadanie udalostí vykonaných na základe pravidiel pre doručenú poštu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313514"
---
# <a name="find-events-performed-on-inbox-rules"></a>Vyhľadanie udalostí vykonaných na základe pravidiel pre doručenú poštu

Po vytvorení, zmene alebo odstránení pravidiel pre doručenú poštu sa udalosti zaznamenajú do denníka auditu. Tu je návod na ich revíziu:

1. Vykonajte jednu z nasledujúcich akcií:
   - V Centrum dodržiavania súladu pre Microsoft 365 prejdite <https://compliance.microsoft.com> na položku  \> **Audit riešenia.** Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portáli Microsoft 365 Defender prejdite <https://security.microsoft.com> na položku **Audit**. Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://security.microsoft.com/auditlogsearch> .

    **Poznámka:** Ak sa zobrazí upozornenie, že potrebujete zapnúť auditovanie, pokračujte a zapnite ho teraz. Ak táto funkcia nie je zapnutá, výsledky hľadania nebudú môcť získať údaje z predchádzajúcich dátumov.
1. Vyberte pole Aktivity a vyhľadajte aktivity Exchange poštovej schránky a potom vyberte položku New-InboxRule Vytvoriť pravidlo pre doručenú poštu z Outlook Web App. Keď ste hotoví, kliknutím mimo tably minimalizujte tablu Aktivity.
1. Zadajte rozsah dátumov a potom v poli Používatelia vyberte meno používateľa, ktorého chcete preskúmať. Môžete vybrať viac ako jedného používateľa naraz.
1. Vyberte položku Hľadať. Aktivity sa zobrazia v časti Výsledky.
1. Ak chcete zobraziť podrobnosti, vyberte aktivitu a potom vyberte položku Ďalšie informácie. V časti Parametre sa zobrazí názov pravidla, množiny podmienok a akcií, ktoré bude pravidlo pravidlo trvať.

2. Na **karte Hľadať** na stránke **Audit** nakonfigurujte tieto nastavenia:
   - **Rozsah dátumu a času:** Vyberte rozsah dátumu a času v **poliach Začiatok** **a** Koniec.
   - **Aktivity:** Výber položky **Nový-Doručená poštaRule Vytvorenie pravidla pre doručenú poštu Outlook Web App**

3. Po dokončení kliknite na tlačidlo **Hľadať**. Aktivity sa zobrazia na novej **stránke Auditovanie.**

4. Výberom aktivity vo výsledkoch otvorte výlet podrobností. V **časti** Parametre sa zobrazí názov pravidla, množiny podmienok a akcií, ktoré bude pravidlo pravidlo trvať.

Ďalšie informácie nájdete v téme [Prehľadáte denník auditu a preskúmajte bežné problémy technickej podpory.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
