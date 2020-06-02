---
title: Riešenie problémov s inštaláciou DKIM
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
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506789"
---
# <a name="fix-dkim-setup-issues"></a>Riešenie problémov s inštaláciou DKIM

Ak sa vyskytnú problémy umožňujúce DKIM pre vlastnú doménu, postupujte nasledovne:

- Väčšina problémov s inštaláciou DKIM súvisí s nesprávnymi záznamami DNS. Skontrolujte, či je záznam DKIM CNAME **(nie** TXT záznam) správne naformátovaný. Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Po vytvorení alebo aktualizácii záznamov DKIM DNS v hostiteľskej službe DNS pre vašu doménu (zvyčajne registrátora domén) počkajte na propagáciu záznamov DNS.

- Ak nemôžete vytvoriť záznamy DKIM DNS v Centre spravovania, môžete nahradiť \<CustomDomain\> vlastnou doménou (napríklad contoso.com) a spustiť tento príkaz v [prostredí Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
