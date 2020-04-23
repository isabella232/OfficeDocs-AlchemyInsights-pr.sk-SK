---
title: Riešenie problémov s nastavením DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717577"
---
# <a name="fix-dkim-setup-issues"></a>Riešenie problémov s nastavením DKIM

Ak sa vyskytnú problémy umožňujúce DKIM pre vlastnú doménu, použite nasledovný postup:

- Väčšina problémov s nastavením DKIM súvisí s nesprávnymi záznamami DNS. Overte, či záznam DKIM CNAME (**nie** záznam TXT) je správne naformátovaný. Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Po vytvorení alebo aktualizácii záznamov DNS DKIM na hostiteľskú službu DNS pre vašu doménu (typicky, Registrátor domén), počkajte, kým sa záznamy DNS množiť.

- Ak nemôžete vytvoriť DKIM DNS záznamy v admin Center, môžete \<nahradiť customdomain\> s vlastnou doménou (napríklad contoso.com) a spustiť tento príkaz v prostredí [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`
