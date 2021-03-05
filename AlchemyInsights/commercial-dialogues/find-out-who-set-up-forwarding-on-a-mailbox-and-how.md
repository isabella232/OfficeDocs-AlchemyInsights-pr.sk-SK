---
title: Zistite, kto nastavuje preposielanie v poštovej schránke a ako
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483353"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Zistite, kto nastavuje preposielanie v poštovej schránke a ako

Ak bol v poštovej schránke nastavený externý preposielanie, aktivita sa Audituje ako súčasť rutiny typu cmdlet Set-Mailbox. Tu je návod na nájdenie aktivity v denníku auditu:

1. Prejdite na [centrum dodržiavania súladu & zabezpečenia služieb Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Vyberte položku >  **vyhľadávanie denníkov auditu** vyhľadávania.
    > [!NOTE]
    > Ak sa zobrazí oznámenie o tom, že je potrebné zapnúť auditovanie, pokračujte a teraz ho zapnite. Ak táto funkcia nie je zapnutá, výsledky hľadania nebudú môcť vytiahnuť údaje z predchádzajúcich dátumov.
1. Uistite sa, že pole **aktivity** je nastavené na možnosť **Zobraziť výsledky pre všetky aktivity** (predvolené). Zadajte rozsah dátumov. Nemusíte špecifikovať meno používateľa.
1. Vyberte položku **Hľadať**. Aktivity sa zobrazia v časti **výsledky**.
1. Vyberte položku **výsledky filtrovania** a potom do poľa Filter **aktivity** zadajte položku **množina poštových schránok** . Tým sa vrátia všetky aktivity v **nastaveniach poštovej schránky** .
1. Ak chcete zobraziť podrobnosti, vyberte aktivitu a potom vyberte položku **Ďalšie informácie**. V časti **parametre** môžete zobraziť e-mailovú adresu preposielania, ktorá bola nastavená v poštovej schránke. **Userid** označuje používateľa, ktorý v poštovej schránke nastavil externý preposielanie.
Ďalšie informácie nájdete v téme [vyhľadávanie v denníku auditu služieb Office 365 na riešenie bežných scenárov](https://go.microsoft.com/fwlink/?linkid=2103944).