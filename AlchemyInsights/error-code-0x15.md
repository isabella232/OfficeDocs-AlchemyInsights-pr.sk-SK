---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ak sa pri aktivácii balíka Office 2013 na nasadenie služieb vzdialenej pracovnej plochy (RDS) zobrazuje chyba, zvážte povolenie adalu úpravou databázy Registry.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506861"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Chyba pri aktivácii balíka Office 2013 v službách vzdialenej pracovnej plochy

Ak sa pri aktivácii balíka Office 2013 na nasadenie služieb vzdialenej pracovnej plochy (RDS) zobrazuje chyba, zvážte povolenie adalu úpravou databázy Registry.
  
|**Kľúč databázy Registry**|**Typ**|**Hodnota**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Ďalšie informácie sa nachádzajú v téme [Povolenie moderného overovania balíka Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL je predvolene zapnutá v aplikáciách Microsoft 365 pre podniky a Office 2016. Služby vzdialenej pracovnej plochy (RDS) sa predtým nazývali terminálové služby.
  