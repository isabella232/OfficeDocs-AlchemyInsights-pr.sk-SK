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
description: Ak sa pri aktivácii balíka Office 2013 v nasadeniach služieb vzdialenej pracovnej plochy zobrazí chyba, zvážte povolenie ADAL úpravou databázy Registry.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316701"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Chyba pri aktivácii Office 2013 v službách vzdialenej pracovnej plochy

Ak sa pri aktivácii balíka Office 2013 v nasadeniach služieb vzdialenej pracovnej plochy zobrazí chyba, zvážte povolenie ADAL úpravou databázy Registry.
  
|**Kľúč databázy Registry**|**Typ**|**Hodnota**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Ďalšie informácie nájdete v téme [Povolenie moderného overovania pre Office 2013 v Windows zariadeniach.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Poznámka:** ADAL je vo Windowse Aplikácie Microsoft 365 pre veľké organizácie a Office 2016 predvolene povolená. Služby vzdialenej pracovnej plochy sa predtým nazývali Terminálové služby.
  