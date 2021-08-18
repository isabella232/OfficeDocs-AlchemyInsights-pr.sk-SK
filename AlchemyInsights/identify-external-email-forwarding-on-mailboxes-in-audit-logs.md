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
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899899"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Určenie, kedy je v poštových schránkach nakonfigurované preposielanie externých e-mailov

Keď používateľ Microsoft 365 externý preposielanie e-mailov v poštovej schránke, aktivita sa audituje ako súčasť rutiny typu cmdlet **Set-Mailbox.** Aktivitu môžete zobraziť pomocou vyhľadávania denníka auditu. Tu je postup.

1. Vykonajte niektorý z týchto krokov:
   - V Centrum dodržiavania súladu pre Microsoft 365 prejdite <https://compliance.microsoft.com> na položku  \> **Audit riešení.** Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portáli Microsoft 365 Defender prejdite <https://security.microsoft.com> na položku **Audit**. Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://sip.security.microsoft.com/auditlogsearch> .

2. Na stránke **Audit** overte, či **je vybratá** karta Hľadať, a potom nakonfigurujte tieto nastavenia:
   - Vyberte rozsah dátumu a času v **poliach Začiatok** **a** Koniec.
   - **Overte, či** pole Aktivity **obsahuje položku Zobraziť výsledky pre všetky aktivity.**

3. Po dokončení kliknite na tlačidlo **Hľadať**. Aktivity sa zobrazia na novej **stránke Auditovanie.**

4. Vo výsledkoch kliknite na položku **Filtrovať výsledky** a do poľa filtra aktivity zadajte text **Set-Mailbox.**

5. Vo výsledkoch vyberte záznam auditu. Na **letáku** Podrobnosti kliknite na položku **Ďalšie informácie**. Ak chcete zistiť, či aktivita súvisí s preposielanie e-mailov, musíte si pozrieť podrobnosti každého záznamu auditu.

   - **ObjectId:** Hodnota aliasu poštovej schránky, ktorá bola upravená.
   - **Parametre:** _ForwardingSmtpAddress označuje_ cieľovú e-mailovú adresu.
   - **UserId:** Používateľ, ktorý nakonfiguroval preposielanie e-mailov v poštovej schránke **v poli ObjectId.**

Ďalšie informácie nájdete v téme Určenie [osoby, ktorá nastavila preposielanie e-mailov v poštovej schránke.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
