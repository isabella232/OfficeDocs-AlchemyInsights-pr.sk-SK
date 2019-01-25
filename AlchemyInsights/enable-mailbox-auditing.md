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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500297"
---
# <a name="enable-mailbox-auditing"></a>Povoliť auditovanie poštovej schránky

Povoliť auditovanie poštovej schránky pre jedného používateľa alebo celú organizáciu nasledujúce rutiny cmdlet je nutné spustiť z vzdialené prostredie PowerShell:
  
 **Jedného používateľa**
  
Set-Mailbox - Identity "Jane Dow" - AuditEnabled $true
  
 Organization
  
Get-Mailbox - ResultSize Unlimited - Filter {RecipientTypeDetails - eq "UserMailbox"} | Nastaviť poštové schránky - AuditEnabled $true
  
Ďalšie informácie
  

