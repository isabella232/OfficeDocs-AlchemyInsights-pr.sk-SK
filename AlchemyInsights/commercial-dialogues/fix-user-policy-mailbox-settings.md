---
title: Oprava nastavení politiky používateľa/poštovej schránky
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034733"
---
# <a name="fix-user-policymailbox-settings"></a>Oprava nastavení politiky používateľa/poštovej schránky

Toto hlásenie sa týka nastavení nevyžiadanej pošty v poštovej schránke. Ak chcete skontrolovať nastavenia, vykonajte nasledovné kroky:

1. Spustite Exchange Management Shell. Ďalšie informácie nájdete v téme [Otvorenie Exchange správy e-Exchange.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Spustite tento príkaz (pomocou e-mailovej adresy používateľa):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Skontrolujte, či je e-mailová adresa odosielateľa súčasťou **trustedSendersAndDomains** alebo **BlockedSendersAndDomains.** Ak sa e-mailová adresa nachádza v jednom zo zoznamov, možno ju budete musieť odstrániť. Ďalšie informácie nájdete v téme [Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
