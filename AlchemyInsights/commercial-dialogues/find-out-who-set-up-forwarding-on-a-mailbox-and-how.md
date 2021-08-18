---
title: Zistite, kto nastavil preposielanie poštovej schránky a ako
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317823"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Zistite, kto nastavil preposielanie poštovej schránky a ako

Ak bolo v poštovej schránke nastavené externé preposielanie, aktivita sa audituje ako súčasť rutiny typu cmdlet **Set-Mailbox.** Tu je postup, ako nájsť aktivitu v denníku auditu:

1. Vykonajte jednu z nasledujúcich akcií:
   - V Centrum dodržiavania súladu pre Microsoft 365 prejdite <https://compliance.microsoft.com> na položku  \> **Audit riešenia.** Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portáli Microsoft 365 Defender prejdite <https://security.microsoft.com> na položku **Audit**. Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://security.microsoft.com/auditlogsearch> .

   **Poznámka:** Ak sa zobrazí upozornenie, že potrebujete zapnúť auditovanie, pokračujte a zapnite ho teraz. Ak táto funkcia nie je zapnutá, výsledky hľadania nebudú môcť získať údaje z predchádzajúcich dátumov.

2. Na stránke **Audit** overte, či **je vybratá** karta Hľadať, a potom nakonfigurujte tieto nastavenia:
   - Vyberte rozsah dátumu a času v **poliach Začiatok** **a** Koniec.
   - **Overte, či** pole Aktivity **obsahuje položku Zobraziť výsledky pre všetky aktivity.**

3. Po dokončení kliknite na tlačidlo **Hľadať**. Aktivity sa zobrazia na novej **stránke Auditovanie.**

4. Vo výsledkoch kliknutím na stĺpec **Aktivita zoraďte** výsledky a vyhľadajte položky **položky Nastaviť poštovú** schránku.

5. Výberom aktivity vo výsledkoch otvorte výlet podrobností. Ak chcete zistiť, či aktivita súvisí s preposielanie e-mailov, musíte si pozrieť podrobnosti každého záznamu auditu:
   - **ObjectId:** Hodnota aliasu poštovej schránky, ktorá bola upravená.
   - **Parametre:** _ForwardingSmtpAddress označuje_ cieľovú e-mailovú adresu.
   - **UserId:** Používateľ, ktorý nakonfiguroval preposielanie e-mailov v poštovej schránke **v poli ObjectId.**

Ďalšie informácie nájdete v téme Určenie [osoby, ktorá nastavila preposielanie e-mailov v poštovej schránke.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
