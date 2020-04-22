---
title: Oprava problémov s doručením e-mailov verejným priečinkom s podporou e-mailu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716367"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Oprava problémov s doručením e-mailov verejným priečinkom s podporou e-mailu

Ak externí odosielatelia nemôžu odosielať správy do verejných priečinkov s podporou e-mailu a odosielatelia dostanú chybu: **Nepodarilo sa nájsť (550 5.4.1)**, overte, či je doména e-mailu pre verejný priečinok nakonfigurovaná ako doména interného prenosu namiesto autoritatívnej domény:

1. Otvorte [Exchange Admin Center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Prejsť na **mail flow** \> **akceptované**domény, vyberte akceptovanú doménu, a potom kliknite na tlačidlo **Upraviť**.

3. Na stránke vlastnosti, ktorá sa otvorí, ak je typ domény nastavený na **autoritatívny**, zmeňte hodnotu na **interný Relay** a potom kliknite na tlačidlo **Uložiť**.

Ak externí odosielatelia dostanú chybu nemáte **povolenie (550 5.7.13)**, spustite nasledujúci príkaz v [službe Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) vidieť povolenia pre anonymných používateľov vo verejnom priečinku:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Napríklad `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Umožniť externým používateľom odosielať e-maily do tohto verejného priečinka, pridajte CreateItems prístup právo na anonymný používateľ. Napríklad `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
