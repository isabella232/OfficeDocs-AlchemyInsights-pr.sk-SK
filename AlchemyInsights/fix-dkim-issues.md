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
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744965"
---
# <a name="fix-dkim-setup-issues"></a>Riešenie problémov s nastavením DKIM

Ak sa vyskytnú problémy s povolením DKIM pre vlastnú doménu, postupujte takto:

- Väčšinu problémov s nastavením DKIM súvisia s nesprávnymi záznamami DNS. Overte, či je záznam CNAME CNAME (**nie** txt záznam) naformátovaný správne. Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Po vytvorení alebo aktualizácii DNS záznamov v hostiteľskej službe DNS pre svoju doménu (zvyčajne registrátora domén) počkajte, kým sa DNS záznamy rozšíria.

- Ak nie je možné vytvoriť DNS záznamy DKIM v centre spravovania, môžete nahradiť \<CustomDomain\> svoju vlastnú doménu (napríklad contoso.com) a spustiť tento príkaz v [prostredí Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
