---
title: Oprava politiky pripojenia
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988149"
---
# <a name="fix-connection-policy"></a>Oprava politiky pripojenia

E-mail bol označený ako bezpečný a doručený do priečinka doručenej pošty používateľa, pretože odosielaná IP adresa bola v politike filtra pripojenia označená ako bezpečná. Ak si chcete politiku prekontrolovať, vykonajte tieto kroky:

1. Prejdite do Centra [Office 365 zabezpečenia & a](https://go.microsoft.com/fwlink/p/?linkid=2077143)potom prejdite na položku Politika správy **hrozieb**  >    >  [– ochrana pred nevyžiadanou poštou](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na karte **Vlastné** vyberte politiku filtra **Pripojenie a** potom vyberte položku **Upraviť politiku**.
3. Pozrite si **zoznam povolených IP** adries. Zistite, **Trezor zoznam povolený.**

    > [!NOTE]
    > Spoločnosť Microsoft má predplatné na zdroje dôveryhodných odosielateľov tretích strán. Ak **Trezor zoznamu** povolený, títo dôveryhodní odosielatelia omylom nie sú označení ako nevyžiadaná pošta. Odporúčame vybrať túto možnosť, pretože sa zníži počet nesprávne pozitívnych e-mailov ( dobrej pošty, ktorá sa klasifikuje ako nevyžiadaná pošta), ktorú dostanete.
