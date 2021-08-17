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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882650"
---
# <a name="find-events-performed-on-inbox-rules"></a>Vyhľadanie udalostí vykonaných na základe pravidiel pre doručenú poštu

Po vytvorení, zmene alebo odstránení pravidiel pre doručenú poštu sa udalosti zaznamenajú do denníka auditu. Tu je návod na ich revíziu:

1. Vykonajte jednu z nasledujúcich akcií:
   - V Centrum dodržiavania súladu pre Microsoft 365 prejdite <https://compliance.microsoft.com> na položku  \> **Audit riešení.** Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portáli Microsoft 365 Defender prejdite <https://security.microsoft.com> na položku **Audit**. Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Ak sa zobrazí upozornenie, že potrebujete zapnúť auditovanie, pokračujte a zapnite ho teraz. Ak táto funkcia nie je zapnutá, výsledky hľadania nebudú môcť získať údaje z predchádzajúcich dátumov.

2. Na **karte Hľadať** na stránke **Audit** nakonfigurujte tieto nastavenia:
   - **Rozsah dátumu a času:** Vyberte rozsah dátumu a času v **poliach Začiatok** **a** Koniec.
   - **Aktivity:** Výber položky **Nový-Doručená poštaRule Vytvorenie pravidla pre doručenú poštu Outlook Web App**

3. Po dokončení kliknite na tlačidlo **Hľadať**. Aktivity sa zobrazia na novej **stránke Auditovanie.**

4. Výberom aktivity vo výsledkoch otvorte výlet podrobností. V **časti** Parametre sa zobrazí názov pravidla, množiny podmienok a akcií, ktoré bude pravidlo pravidlo trvať.

Ďalšie informácie nájdete v téme [Prehľadáte denník auditu a preskúmajte bežné problémy technickej podpory.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
