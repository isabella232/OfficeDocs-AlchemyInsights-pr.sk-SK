---
title: Riešenie problémov s nastavením DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945946"
---
# <a name="fix-dkim-setup-issues"></a>Riešenie problémov s nastavením DKIM

Ak sa vyskytnú problémy pri zapnutí DKIM pre vlastnú doménu, postupujte takto:

- Väčšina problémov s nastavením DKIM súvisí s nesprávnymi DNS záznamami. Overte, či je CNAME záznam DKIM **(nie** TXT záznam) správne naformátovaný. Ďalšie informácie nájdete v tejto [téme.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Po vytvorení alebo aktualizácii DNS záznamov DKIM v hostiteľskej službe DNS pre vašu doménu (zvyčajne je to registrátor domén) počkajte, kým sa DNS záznamy budú šíriť.

- Ak nemôžete vytvoriť DNS záznamy DKIM v centre spravovania, môžete ho nahradiť vlastnou doménou (napríklad contoso.com) a tento príkaz spustiť v \<CustomDomain\> [prostredí Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
