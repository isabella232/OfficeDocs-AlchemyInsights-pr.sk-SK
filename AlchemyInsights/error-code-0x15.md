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
description: Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na nasadenie služby vzdialenej skúsenosti s prácou s počítačom (RDS), zvážte povolenie ADAL úpravou databázy Registry.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703153"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Chyba pri aktivácii balíka Office 2013 služby vzdialenej skúsenosti s prácou s počítačom

Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na nasadenie služby vzdialenej skúsenosti s prácou s počítačom (RDS), zvážte povolenie ADAL úpravou databázy Registry.
  
|**Kľúč databázy Registry**|**Typ**|**Hodnota**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Ďalšie informácie nájdete v časti [povolenie moderného overovania pre balík Office 2013 v zariadeniach so systémom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL je predvolene zapnutá v Microsoft 365 aplikácie pre podniky a Office 2016. Služby vzdialenej pracovnej plochy (RDS) sa predtým pomenovali terminálové služby.
  