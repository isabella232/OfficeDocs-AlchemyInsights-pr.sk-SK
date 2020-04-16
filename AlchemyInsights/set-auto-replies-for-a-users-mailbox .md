---
title: Nastavenie automatických odpovedí pre poštovú schránku používateľa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506647"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Nastavenie automatických odpovedí pre poštovú schránku používateľa

**Metóda 1**

1. Prihláste sa na portáli služieb Office 365.

2. Prejdite na položky **Používatelia > Aktívni používatelia** (alebo **Skupiny > Zdieľané poštové schránky**, ak to nastavujete v zdieľanej poštovej schránke).

3. Vyberte používateľa, ktorý má poštovú schránku servera Microsoft Exchange.

4. V rozbaľovacej ponuke na pravej strane prejdite na položky **Nastavenia pošty > Automatické odpovede** (ak ide o zdieľanú poštovú schránku, stačí kliknúť na položku **Automatické odpovede** v rozbaľovacej ponuke).

**Metóda 2**

1. Prihláste sa na portáli pre správcov služieb Office 365 pomocou prihlasovacích údajov správcu.

2. Rozbaľte ponuku **Centrá spravovania** a potom kliknite na položku **Exchange**.

3. Kliknite na obrázok v pravom hornom rohu, kliknite na položku **Iný používateľ** a potom vyberte poštovú schránku používateľa, ktorú chcete zmeniť.

4. Na ľavej strane vyberte položku **Možnosti**, kliknite na položku **Organizovať e-mail** a potom kliknite na položku **Automatické odpovede.**

**Metóda 3**

Spustite nasledujúcu rutinu typu cmdlet v prostredí Exchange Online PowerShell:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

Ďalšie informácie o tejto rutine typu cmdlet nájdete v téme [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
