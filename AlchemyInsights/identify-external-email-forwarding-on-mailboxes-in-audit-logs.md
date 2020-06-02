---
title: Identifikácia externého posielania e-mailov ďalej v poštových schránkach v denníkoch auditu
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
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508967"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifikácia, keď je externé presmerovanie e-mailov nakonfigurované v poštových schránkach

Keď používateľ Microsoft 365 nakonfiguruje externé e-mail presmerovanie poštovej schránky, činnosť je auditovaný ako súčasť rutiny cmdlet **Set-Mailbox** . Aktivitu môžete zobraziť pomocou vyhľadávania denníka auditu v Centre zabezpečenia & súladu.

1. Prihláste sa do Centra [& zabezpečenia spoločnosti Microsoft 365](https://protection.office.com/).

2. Prejdite na stránku **vyhľadávania**  >  **v denníku auditu.**

3. Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Koncový dátum.** Nie je potrebné zadať meno používateľa. Skontrolujte, či je pole **Aktivity** nastavené na **možnosť Zobraziť výsledky pre všetky aktivity**.

4. Kliknite na tlačidlo **Hľadať**.

Vo výsledkoch kliknite na **položku Filtrovať výsledky** a do poľa filter aktivity zadajte text **Nastaviť poštovú schránku.** Vo výsledkoch vyberte záznam auditu. V rozbaľovacom zozname **Podrobnosti** kliknite na položku **Ďalšie informácie**. Ak chcete zistiť, či aktivita súvisí s posielaním e-mailov ďalej, musíte sa pozrieť na podrobnosti každého záznamu auditu.

- **ObjectId:** Hodnota aliasu poštovej schránky, ktorá bola upravená.

- **Parametre**: _ForwardingSmtpAddress_ označuje cieľovú e-mailovú adresu.

- **UserId:** Používateľ, ktorý nakonfiguroval e-mail presmerovanie v poštovej schránke v **objectid** pole.

Ďalšie informácie sa nachádzajú v téme [Určenie osôb, ktoré nastavia preposielanie e-mailov pre poštovú schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
