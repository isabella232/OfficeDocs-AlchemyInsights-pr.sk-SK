---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402754"
---
Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry. 
  
|**Kľúč databázy Registry**|**Typ**|**Hodnota**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Ďalšie informácie, pozrite si [Umožňujú moderné overenie Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL zapnutá v predvolenom nastavení Office 365 ProPlus a Office 2016. > remote Desktop Services (RDS) bol predtým pomenovaný terminálových služieb. 
  

