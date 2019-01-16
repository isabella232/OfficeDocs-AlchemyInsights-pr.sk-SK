---
title: Povoliť auditovanie poštovej schránky
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28310593"
---
# <a name="enable-mailbox-auditing"></a>Povoliť auditovanie poštovej schránky

Povoliť auditovanie poštovej schránky pre jedného používateľa alebo celú organizáciu nasledujúce rutiny cmdlet je nutné spustiť z vzdialené prostredie PowerShell:
  
 **Jedného používateľa**
  
Set-Mailbox - Identity "Jane Dow" - AuditEnabled $true
  
 **Organization**
  
Get-Mailbox - ResultSize Unlimited - Filter {RecipientTypeDetails - eq "UserMailbox"} | Nastaviť poštové schránky - AuditEnabled $true
  
[Ďalšie informácie](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

