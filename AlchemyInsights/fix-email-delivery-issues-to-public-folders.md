---
title: Riešenie problémov s doručovaním e-mailov do verejných priečinkov s podporou e-mailu
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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366479"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Riešenie problémov s doručovaním e-mailov do verejných priečinkov s podporou e-mailu

Ak externí odosielatelia nedokážu odosielať správy do verejných priečinkov s podporou e-mailu a odosielateľom sa zobrazí chyba: **Nepodarilo sa nájsť (550 5.4.1)**, overte, či je doména e-mailu pre verejný priečinok nakonfigurovaná ako doména interného prenosu namiesto smerodajnej domény:

1. Otvorte [centrum spravovania pre Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Prejdite na **Mail flow** položku \> **akceptované domény**toku pošty, vyberte akceptovanú doménu a potom kliknite na položku **Upraviť**.

3. Na stránke vlastnosti, ktorá sa otvorí, ak je typ domény nastavený na hodnotu **autoritatívne**, zmeňte hodnotu na **interný prenos** a potom kliknite na tlačidlo **Uložiť**.

Ak externým odosielateľom sa zobrazí chyba, **ktorú nemáte povolenie (550 5.7.13)**, spustite nasledujúci príkaz v [prostredí Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a zobrazte povolenia anonymných používateľov vo verejnom priečinku:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Napríklad `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Ak chcete povoliť externým používateľom odosielať e-maily do tohto verejného priečinka, pridajte CreateItems prístup k používateľovi anonymné. Napríklad `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
