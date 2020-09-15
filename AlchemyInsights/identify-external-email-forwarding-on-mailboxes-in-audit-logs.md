---
title: Identifikácia externého preposielania e-mailov poštových schránok v denníkoch auditu
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696312"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Určenie, kedy je externé presmerovanie e-mailov nakonfigurované v poštových schránkach

Keď používateľ programu Microsoft 365 nakonfiguruje externé preposielanie e-mailov v poštovej schránke, aktivita sa Audituje ako súčasť rutiny typu cmdlet **Set-Mailbox** . Aktivitu môžete zobraziť pomocou vyhľadávania denníkov auditu v centre zabezpečenia & dodržiavania súladu.

1. Prihláste sa do [Centra zabezpečenia dodržiavania súladu so službou Microsoft 365 Security &](https://protection.office.com/).

2. Prejdite na stránku **Search**  >  **vyhľadávania denníka auditu** vyhľadávania.

3. V poliach **Počiatočný** dátum a **Koncový dátum** vyberte rozsah dátumov. Nemusíte špecifikovať meno používateľa. Overte, či je pole **aktivity** nastavené na možnosť **Zobraziť výsledky pre všetky aktivity**.

4. Kliknite na položku **Hľadať**.

Vo výsledkoch kliknite na položku **filtrovať výsledky** a do poľa Filter aktivity zadajte výraz **množina poštových schránok** . Vo výsledkoch vyberte záznam auditu. V rozbaľovacom zozname **Podrobnosti** kliknite na položku **Ďalšie informácie**. Ak chcete zistiť, či sa aktivita týka preposielania e-mailov, musíte si pozrieť podrobnosti o každom zázname auditu.

- **ObjectID**: hodnota aliasu v poštovej schránke, ktorá bola upravená.

- **Parametre**: _ForwardingSMTPAddress_ označuje cieľovú e-mailovú adresu.

- **Userid**: používateľ, ktorý nakonfiguroval preposielanie e-mailov v poštovej schránke v poli **objectID** .

Ďalšie informácie nájdete v téme [Určenie používateľov, ktorí nastavujú preposielanie e-mailov pre poštovú schránku](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
