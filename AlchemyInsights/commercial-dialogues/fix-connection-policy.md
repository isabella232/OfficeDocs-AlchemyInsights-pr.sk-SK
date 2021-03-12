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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750601"
---
# <a name="fix-connection-policy"></a>Oprava politiky pripojenia

E-mail bol označený ako bezpečný a doručený do priečinka doručenej pošty používateľa, pretože odosielajúca IP adresa bola v politike filtra pripojenia označená ako bezpečná. Ak chcete skontrolovať politiku, postupujte takto:

1. Prejdite na [centrum dodržiavania súladu pre Office 365 Security &](https://go.microsoft.com/fwlink/p/?linkid=2077143)a potom **prejdite do časti**  >    >  [Ochrana pred nevyžiadanou poštou](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na karte **vlastné** vyberte **politiku filtrovania pripojenia** a potom vyberte položku **upraviť politiku**.
3. Pozrite si zoznam **povolených IP adries** . Skontrolujte, či je povolený **bezpečný zoznam** .

    > [!NOTE]
    > Spoločnosť Microsoft sa prihlási k zdrojom tretích strán dôveryhodných odosielateľov. Ak je povolený **bezpečný zoznam** , títo Dôveryhodní odosielatelia nie sú omylom označení ako nevyžiadaná pošta. Odporúčam vybrať túto možnosť, pretože zníži počet falošných poplachov (dobrá pošta klasifikovaná ako nevyžiadaná pošta), ktorá sa zobrazí.
