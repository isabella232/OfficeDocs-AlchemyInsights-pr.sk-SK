---
title: Odstránenie problémov s doručovaním e-mailov do verejných priečinkov s podporou e-mailu
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
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068827"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Odstránenie problémov s doručovaním e-mailov do verejných priečinkov s podporou e-mailu

Ak externí odosielatelia nemôže odosielať správy do verejných priečinkov s podporou e-mailu a odosielateľom sa zobrazuje chyba: Nepodarilo sa nájsť **(550 5.4.1)**, skontrolujte, či je e-mailová doména verejného priečinka nakonfigurovaná ako doména na interné odosielanie namiesto autoritatívnej domény:

1. Otvorte [Exchange spravovania .](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Prejdite do **časti Tok** \> **pošty Akceptované domény**, vyberte akceptovanú doménu a potom kliknite na položku **Upraviť**.

3. Ak je na stránke vlastností nastavený typ domény Autoritatívny **,** zmeňte hodnotu na Interný prenos **a** potom kliknite na tlačidlo **Uložiť**.

Ak sa externým odosielateľom zobrazí chyba, že nemáte povolenie **(550 5.7.13),** v prostredí [PowerShell spustite nasledujúci](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) príkaz Exchange Online a zobrazte povolenia anonymných používateľov vo verejnom priečinku:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Príklad: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Ak chcete povoliť externým používateľom odosielať e-maily do tohto verejného priečinka, pridajte prístup pomocou položky Vytvoriť Položky priamo používateľovi Anonymné. Príklad: `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
