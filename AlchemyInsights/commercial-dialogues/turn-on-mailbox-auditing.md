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
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058053"
---
# <a name="turn-on-mailbox-auditing"></a>Zapnutie auditovania poštovej schránky

Ak chcete zapnúť auditovanie poštovej schránky pre jedného používateľa alebo celú organizáciu, spustite túto rutinu typu cmdlet v prostredí Remote PowerShell:

- **Jeden používateľ:** Set-Mailbox identity "Jane Dow" -AuditEnabled $true
- **Organizácia:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Ďalšie informácie nájdete v téme Správa [auditovania poštovej schránky.](https://go.microsoft.com/fwlink/?linkid=2103668)