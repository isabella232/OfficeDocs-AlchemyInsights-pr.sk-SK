---
title: Čítanie denníkov auditu pre odstránené udalosti
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324748"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Čítanie denníkov auditu pre odstránené udalosti

Postup:

1. Vykonajte jednu z nasledujúcich akcií:
   - V časti Centrum dodržiavania súladu pre Microsoft 365 prejdite <https://compliance.microsoft.com> na položku **Kontrola** \> **riešení.** Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portáli Microsoft 365 Defender prejdite <https://security.microsoft.com> na položku **Audit**. Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://security.microsoft.com/auditlogsearch> .

    **Poznámka:** Ak sa zobrazí upozornenie, že túto funkciu potrebujete zapnúť, zapnite ju teraz. Ak funkcia nie je zapnutá, výsledky hľadania nebudú môcť získať údaje z predchádzajúcich dátumov.

2. Na **karte Hľadať** na stránke **Audit** nakonfigurujte tieto nastavenia:
   - **Rozsah dátumu a času:** Vyberte rozsah dátumu a času v **poliach Začiatok** **a** Koniec.
   - **Aktivity:** Zadajte **Exchange aktivity poštovej** schránky a potom vyberte tieto hodnoty:
     - **Odstránené správy z priečinka Odstránené položky**
     - **Premiestnené správy do priečinka Odstránené položky**

       Keď ste hotoví, kliknutím mimo tably minimalizujte **tablu** Aktivity.

   - **Používatelia:** Prijmite prázdnu predvolenú hodnotu, aby sa vrátili výsledky pre všetkých používateľov, alebo zadajte jedného alebo viacerých používateľov.

3. Po dokončení kliknite na tlačidlo **Hľadať**. Aktivity sa zobrazia na novej **stránke Auditovanie.**

4. Výberom aktivity vo výsledkoch otvorte výlet podrobností. Ďalšie informácie o odstránenej položke, napríklad predmet a umiestnenie položky v prípade jej odstránení, sa zobrazia v poli **Ovplyvnené Položky.**

   **Poznámka:** Odstránené položky nie je možné obnoviť pomocou funkcie denníka auditu. Ak chcete obnoviť odstránené položky, pozrite si [časť Obnovenie odstránených e-mailových správ Outlook na webe.](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

Ďalšie informácie nájdete v téme [Vyhľadávanie v denníku auditu a preskúmanie bežných problémov technickej podpory.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
