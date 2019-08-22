---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527061"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Chyba pri aktivácii Office 2013 na služby vzdialenej pracovnej plochy

Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.
  
|**Kľúč databázy Registry**|**Typ**|**Hodnota**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Ďalšie informácie, pozrite si [Umožňujú moderné overenie Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL zapnutá v predvolenom nastavení Office 365 ProPlus a Office 2016. Remote Desktop Services (RDS) bol predtým pomenovaný terminálových služieb.
  