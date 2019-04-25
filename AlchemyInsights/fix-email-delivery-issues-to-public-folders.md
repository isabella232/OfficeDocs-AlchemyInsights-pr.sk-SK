---
title: Vyriešiť otázky doručovanie pošty do e-mailu verejných priečinkov
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401457"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Vyriešiť otázky doručovanie pošty do e-mailu verejných priečinkov

Ak externých odosielateľov nemôže odoslať správy na poštové verejné priečinky a odosielateľov Zobraziť chybové hlásenie: **Nepodarilo sa nájsť (550 5.4.1)**, skontrolujte email domény pre verejný priečinok je nakonfigurovaný ako doménu interného prenosu namiesto autoritatívnu doménu:

1. Otvorte [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Prejsť na **tok pošty** \> **akceptovaných domén**, vyberte akceptovanej domény, a potom kliknite na tlačidlo **Upraviť**.

3. Vo vlastnostiach stránky otvorí, ak typ domény nastavená na **Authoritative**, zmeňte hodnotu na **interný prenos** a potom kliknite na tlačidlo **Uložiť**.

Ak externých odosielateľov chyba **nemáte povolenie (550 5.7.13)**, spustite nasledujúci príkaz v [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a zobrazia sa povolenia pre anonymných používateľov vo verejnom priečinku:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Napríklad `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Ak chcete povoliť externým používateľom odosielať e-mailom na tento verejný priečinok, pridať CreateItems prístup priamo k užívateľovi Anonym. Napríklad `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
