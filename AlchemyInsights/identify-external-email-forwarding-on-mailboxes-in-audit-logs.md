---
title: Určiť externé preposielanie na poštové schránky v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909545"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifikovať preposielanie externých e-mailov je nakonfigurovaný poštových schránok

Keď používateľ nakonfiguruje externé preposielanie na poštovú schránku, činnosť je audit ako súčasť rutiny cmdlet **Set-Mailbox** . Môžete vidieť aktivitu pomocou vyhľadávanie denník auditu bezpečnosti & centrum súladu.

1. Prihláste sa do [Centrum Office 365 zabezpečenia & súlad](https://protection.office.com/)

2. Kliknite na položku **vyhľadávanie a vyšetrovanie** a vyberte **Vyhľadávanie denník auditu**.

3. Vyberte rozsah dátumov v poliach **Počiatočný dátum** a **Koncový dátum** . Nemusíte zadať meno používateľa. Overenie **činnosti** pole nastavené na **zobrazenie výsledkov pre všetky činnosti**.

4. Kliknite na tlačidlo **Hľadať**.

Vo výsledkoch kliknite na položku **Filtrovať výsledky** a aktivity filtra poľa zadajte **Set-Mailbox** . Vyberte auditný záznam výsledkov. Rozbaľovacie tlačidlo **Podrobnosti** , kliknite na **viac informácií**. Musíte sa pozrieť na detaily každého záznamu auditu na určenie, či činnosť súvisí preposielanie e-mailov.

- **ObjectId**: hodnotu alias poštovej schránky, ktorá bola upravená.

- **Parametre**: _ForwardingSmtpAddress_ označuje cieľovú e-mailovú adresu.

- **ID užívateľa**: používateľ nakonfigurovaný preposielanie e-mailov v poštovej schránke v poli **ObjectId** .

Pre viac informácií, pozri [určenie kto nastaviť preposielanie pre poštovú schránku](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
