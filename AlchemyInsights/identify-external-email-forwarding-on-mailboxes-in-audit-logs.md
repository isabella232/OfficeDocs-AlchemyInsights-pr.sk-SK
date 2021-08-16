---
title: Identifikácia preposielanie externých e-mailov v poštových schránkach v denníkoch auditu
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028767"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Určenie, kedy je v poštových schránkach nakonfigurované preposielanie externých e-mailov

Keď používateľ Microsoft 365 externý preposielanie e-mailov v poštovej schránke, aktivita sa audituje ako súčasť rutiny typu cmdlet **Set-Mailbox.** Aktivitu môžete zobraziť pomocou vyhľadávania denníka auditu v Centre dodržiavania & zabezpečenia.

1. Prihláste sa do [Centra Microsoft 365 súladu](https://protection.office.com/).

2. Prejdite na stránku **vyhľadávania denníka**  >  **auditu vyhľadávania.**

3. Vyberte rozsah dátumov v **poliach Počiatočný dátum** **a Dátum ukončenia.** Meno používateľa nie je potrebné zadať. Skontrolujte, **či je** pole Aktivity nastavené na hodnotu Zobraziť výsledky pre všetky **aktivity.**

4. Kliknite na **tlačidlo Hľadať**.

Vo výsledkoch kliknite na položku **Filtrovať výsledky** a do poľa filtra aktivity zadajte text **Set-Mailbox.** Vo výsledkoch vyberte záznam auditu. Na **letáku** Podrobnosti kliknite na položku **Ďalšie informácie**. Ak chcete zistiť, či aktivita súvisí s preposielanie e-mailov, musíte si pozrieť podrobnosti každého záznamu auditu.

- **ObjectId:** Hodnota aliasu poštovej schránky, ktorá bola upravená.

- **Parametre:** _ForwardingSmtpAddress označuje_ cieľovú e-mailovú adresu.

- **UserId:** Používateľ, ktorý nakonfiguroval preposielanie e-mailov v poštovej schránke **v poli ObjectId.**

Ďalšie informácie nájdete v téme Určenie [osoby, ktorá nastavila preposielanie e-mailov v poštovej schránke.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
