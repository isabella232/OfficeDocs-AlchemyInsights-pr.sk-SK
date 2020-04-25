---
title: Nastavenie automatických odpovedí pre poštovú schránku
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
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788897"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Nastavenie automatických odpovedí pre poštovú schránku používateľa

**Metóda 1**

1. Prihláste sa na portáli služby Microsoft 365.

2. Prejdite na položky **Používatelia > Aktívni používatelia** (alebo **Skupiny > Zdieľané poštové schránky**, ak to nastavujete v zdieľanej poštovej schránke).

3. Vyberte používateľa, ktorý má poštovú schránku servera Microsoft Exchange.

4. V rozbaľovacej ponuke na pravej strane prejdite na položky **Nastavenia pošty > Automatické odpovede** (ak ide o zdieľanú poštovú schránku, stačí kliknúť na položku **Automatické odpovede** v rozbaľovacej ponuke).

**Metóda 2**

1. Prihláste sa na portáli pre správcov služby Microsoft 365 pomocou prihlasovacích údajov správcu.

2. Rozbaľte ponuku **Centrá spravovania** a potom kliknite na položku **Exchange**.

3. Kliknite na obrázok v pravom hornom rohu, kliknite na položku **Iný používateľ** a potom vyberte poštovú schránku používateľa, ktorú chcete zmeniť.

4. Na ľavej strane vyberte položku **Možnosti**, kliknite na položku **Organizovať e-mail** a potom kliknite na položku **Automatické odpovede.**

**Metóda 3**

Spustite nasledujúcu rutinu typu cmdlet v prostredí Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Ďalšie informácie o tejto rutine typu cmdlet nájdete v téme [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
