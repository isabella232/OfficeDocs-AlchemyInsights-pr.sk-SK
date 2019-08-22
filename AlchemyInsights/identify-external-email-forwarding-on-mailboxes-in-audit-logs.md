---
title: Určiť externé preposielanie na poštové schránky v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539116"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifikovať preposielanie externých e-mailov je nakonfigurovaný poštových schránok

Keď používateľ Office 365 konfiguruje externé preposielanie na poštovú schránku, činnosť je audit ako súčasť rutiny cmdlet **Set-Mailbox** . Môžete vidieť aktivitu pomocou vyhľadávanie denník auditu bezpečnosti & centrum súladu.

1. Prihláste sa do [Centrum Office 365 zabezpečenia & súladu](https://protection.office.com/).

2. Prejdite na **vyhľadávanie** > stránka**vyhľadávanie denník auditu** .

3. Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Koncový dátum** . Nemusíte zadať meno používateľa. Overenie **činnosti** pole nastavené na **zobrazenie výsledkov pre všetky činnosti**.

4. Kliknite na tlačidlo **Hľadať**.

Vo výsledkoch kliknite na položku **Filtrovať výsledky** a aktivity filtra poľa zadajte **Set-Mailbox** . Vyberte auditný záznam výsledkov. Rozbaľovacie tlačidlo **Podrobnosti** , kliknite na **viac informácií**. Musíte sa pozrieť na detaily každého záznamu auditu na určenie, či činnosť súvisí preposielanie e-mailov.

- **ObjectId**: hodnotu alias poštovej schránky, ktorá bola upravená.

- **Parametre**: _ForwardingSmtpAddress_ označuje cieľovú e-mailovú adresu.

- **ID užívateľa**: používateľ nakonfigurovaný preposielanie e-mailov v poštovej schránke v poli **ObjectId** .

Pre viac informácií, pozri [určenie kto nastaviť preposielanie pre poštovú schránku](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
