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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988225"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Zistite, kto nastavil preposielanie poštovej schránky a ako

Ak bolo v poštovej schránke nastavené externé preposielanie, aktivita sa audituje ako súčasť rutiny Set-Mailbox cmdlet. Tu je postup, ako nájsť aktivitu v denníku auditu:

1. Prejdite do Centra [Office 365 zabezpečenia & súladu.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Vyberte **položku Vyhľadávanie** v >  **denníku auditu.**
    > [!NOTE]
    > Ak sa zobrazí upozornenie, že potrebujete zapnúť auditovanie, pokračujte a zapnite ho teraz. Ak táto funkcia nie je zapnutá, výsledky hľadania nebudú môcť získať údaje z predchádzajúcich dátumov.
1. Uistite **sa, že** pole Aktivity je **nastavené na možnosť Zobraziť výsledky pre všetky aktivity** (predvolené). Zadajte rozsah dátumov. Meno používateľa nie je potrebné zadať.
1. Vyberte **položku Hľadať**. Aktivity sa zobrazia v časti **Výsledky.**
1. Vyberte **položku Filtrovať** výsledky a potom do **poľa Filter aktivít** zadajte nastavenie **poštovej** schránky. Vrátia sa všetky **aktivity súvisiace s nastavením poštovej** schránky.
1. Ak chcete zobraziť podrobnosti, vyberte aktivitu a potom vyberte položku **Ďalšie informácie**. V **časti Parametre** sa zobrazí e-mailová adresa na preposielanie správ, ktorá bola nastavená v poštovej schránke. The **UserID** predstavuje používateľa, ktorý nastavil externé preposielanie v poštovej schránke.
Ďalšie informácie nájdete v téme [Riešenie bežných Office 365 vyhľadávaní v denníku auditu.](https://go.microsoft.com/fwlink/?linkid=2103944)