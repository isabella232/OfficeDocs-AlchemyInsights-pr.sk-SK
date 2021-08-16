---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ak sa pri aktivácii aplikácie Office 2013 v nasadeniach služieb vzdialenej pracovnej plochy zobrazí chyba, zvážte povolenie služby ADAL úpravou databázy Registry.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100777"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Chyba pri aktivácii Office 2013 v službách vzdialenej pracovnej plochy

Ak sa pri aktivácii aplikácie Office 2013 v nasadeniach služieb vzdialenej pracovnej plochy zobrazí chyba, zvážte povolenie služby ADAL úpravou databázy Registry.
  
|**Kľúč databázy Registry**|**Typ**|**Hodnota**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Ďalšie informácie nájdete v téme [Povolenie moderného overovania pre Office 2013 v Windows zariadeniach.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL je vo Windowse 2016 Aplikácie Microsoft 365 pre veľké organizácie Office predvolene povolená. Služby vzdialenej pracovnej plochy sa predtým nazývali Terminálové služby.
  