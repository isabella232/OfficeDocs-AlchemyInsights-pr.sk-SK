---
title: Odosielateľ neprijíma e-maily odoslané do skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872148"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Odosielateľ neprijíma e-maily odoslané do skupiny Microsoft 365

Na základe predvoleného nastavenia odosielateľ e-mailovej správy do skupiny Microsoft 365 nedostane kópiu správy do priečinka Doručená pošta, a to ani v prípade, že je odosielateľ členom skupiny.

Pomocou tohto príkazu EXO PowerShell môžete odosielateľovi povoliť príjem kópie všetkých e-mailov odoslaných do skupiny Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Ak chcete povoliť nastavenie pre všetky poštové schránky naraz:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Poznámka:** Zmeny tohto nastavenia trvať až hodinu, kým sa prejavia.