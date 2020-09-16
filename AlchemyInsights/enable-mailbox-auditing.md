---
title: Povolenie auditovania poštovej schránky
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806306"
---
# <a name="enable-mailbox-auditing"></a>Povolenie auditovania poštovej schránky

Ak chcete povoliť auditovanie poštovej schránky pre jedného používateľa alebo celú organizáciu, je potrebné spustiť nasledovné rutiny typu cmdlet z vzdialeného sieťového rozhrania:
  
 **Jeden používateľ**
  
Množina poštových schránok – identita "Jane Dow" – AuditEnabled $true
  
 **Organizácie**
  
Get-Mailbox-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Množina poštových schránok – AuditEnabled $true
  
[zistiť viac](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

