---
title: Oprava nastavení politiky používateľa alebo poštovej schránky
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750562"
---
# <a name="fix-user-policymailbox-settings"></a>Oprava nastavení politiky používateľa alebo poštovej schránky

Nastavenia nevyžiadanej pošty v poštovej schránke ovplyvnili túto správu. Ak chcete skontrolovať nastavenia, postupujte takto:

1. Spustite prostredie Exchange Management Shell. Ďalšie informácie nájdete v téme [Otvorenie prostredia Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Spustite tento príkaz (s použitím e-mailovej adresy používateľa):  **Get-mailboxjunkmailconfiguration-identity "user@domain.com"**
3. Skontrolujte, či je e-mailová adresa odosielateľa súčasťou **TrustedSendersAndDomains** alebo **BlockedSendersAndDomains**. Ak sa e-mailová adresa nachádza v niektorom zo zoznamov, možno ju budete musieť odstrániť. Ďalšie informácie nájdete v téme [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
