---
title: Vyriešiť otázky doručovanie pošty do e-mailu verejných priečinkov
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525147"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Vyriešiť otázky doručovanie pošty do e-mailu verejných priečinkov

Ak externých odosielateľov nemôže odoslať správy na poštové verejné priečinky a odosielateľov Zobraziť chybové hlásenie: **Nepodarilo sa nájsť (550 5.4.1)**, skontrolujte email domény pre verejný priečinok je nakonfigurovaný ako doménu interného prenosu namiesto autoritatívnu doménu:

1. Otvorte [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Prejsť na **tok pošty** \> **akceptovaných domén**, vyberte akceptovanej domény, a potom kliknite na tlačidlo **Upraviť**.

3. Vo vlastnostiach stránky otvorí, ak typ domény nastavená na **Authoritative**, zmeňte hodnotu na **interný prenos** a potom kliknite na tlačidlo **Uložiť**.

Ak externých odosielateľov chyba **nemáte povolenie (550 5.7.13)**, spustite nasledujúci príkaz v [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a zobrazia sa povolenia pre anonymných používateľov vo verejnom priečinku:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Napríklad `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Ak chcete povoliť externým používateľom odosielať e-mailom na tento verejný priečinok, pridať CreateItems prístup priamo k užívateľovi Anonym. Napríklad `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
