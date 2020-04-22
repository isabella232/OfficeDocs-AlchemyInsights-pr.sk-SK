---
title: Identifikujte externé posielanie e-mailov v poštových schránkach v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716475"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifikovať, keď externý e-mail presmerovanie je nakonfigurovaný na poštové schránky

Keď používateľ Microsoft 365 nakonfiguruje externý e-mail forwarding na poštovú schránku, aktivita je auditovaný ako súčasť rutiny cmdlet **Set-Mailbox** . Aktivitu môžete vidieť pomocou vyhľadávania denníka auditu v centre zabezpečenia & Compliance Center.

1. Prihláste sa do [Microsoft 365 Security & centrum súladu](https://protection.office.com/).

2. Prejdite na stránku vyhľadávania**denníka auditu** **vyhľadávania** > .

3. Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Dátum ukončenia** . Nie je potrebné zadať používateľské meno. Overte, či je pole **aktivity** nastavené na **zobrazenie výsledkov pre všetky aktivity**.

4. Kliknite na tlačidlo **Hľadať**.

Vo výsledkoch kliknite na položku **výsledky filtrovania** a zadajte do poľa Filter aktivity pole **nastaviť poštovú schránku** . Vo výsledkoch vyberte záznam auditu. V rozbaľovacom zozname **Podrobnosti** kliknite na položku **Ďalšie informácie**. Ak chcete zistiť, či aktivita súvisí s posielaním e-mailov, musíte sa pozrieť na Podrobnosti každého záznamu auditu.

- **ObjectID**: alias hodnota poštovej schránky, ktorá bola zmenená.

- **Parametre**: _ForwardingSMTPAddress_ označuje cieľovú e-mailovú adresu.

- **Userid**: používateľ, ktorý nakonfiguroval presmerovanie e-mailov na poštovú schránku v poli **objectID** .

Ďalšie informácie nájdete v téme [určenie, kto nastaviť presmerovanie e-mailov pre poštovú schránku](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
