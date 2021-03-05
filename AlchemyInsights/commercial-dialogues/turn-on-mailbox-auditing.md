---
title: Zapnutie auditovania poštovej schránky
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483543"
---
# <a name="turn-on-mailbox-auditing"></a>Zapnutie auditovania poštovej schránky

Ak chcete zapnúť auditovanie poštovej schránky pre jedného používateľa alebo celú organizáciu, spustite nasledujúce rutiny typu cmdlet z vzdialeného prostredia PowerShell:

- **Jeden používateľ**: Set-Mailbox identita "Jane Dow" – AuditEnabled $True
- **Organizácia**: Get-Mailbox-ResultSize Unlimited-filter {recipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox – AuditEnabled $true

Ďalšie informácie nájdete v téme [Spravovanie auditovania poštovej schránky](https://go.microsoft.com/fwlink/?linkid=2103668).