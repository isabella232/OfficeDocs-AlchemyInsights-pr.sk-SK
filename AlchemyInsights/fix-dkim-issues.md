---
title: Opraviť problémy s inštaláciou DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765395"
---
# <a name="fix-dkim-setup-issues"></a>Opraviť problémy s inštaláciou DKIM

Ak sa vyskytnú problémy, umožňujúce DKIM pre vlastnú doménu, použite nasledujúce kroky:

- Väčšina problémov s nastavením DKIM súvisia s nesprávne záznamy DNS. Overte, či záznam DKIM CNAME (**nie** záznam TXT) je správne naformátované. Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Po vytvorení alebo aktualizovať záznamy DKIM DNS v hostiteľskej služby DNS pre vašu doménu (zvyčajne registrátora domény), čakať na DNS záznamy na propagáciu.

- Ak nemôžete vytvoriť DKIM DNS záznamy admin Center, môžete nahradiť \<CustomDomain\> s svoje vlastné domény (napríklad contoso.com) a spustite tento príkaz v [Online PowerShell výmeny](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
