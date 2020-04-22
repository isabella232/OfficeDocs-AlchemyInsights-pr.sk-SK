---
title: Povoliť auditovanie poštových schránok
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703586"
---
# <a name="enable-mailbox-auditing"></a>Povoliť auditovanie poštových schránok

Ak chcete povoliť auditovanie poštových schránok pre jedného používateľa alebo celú organizáciu, musíte spustiť nasledujúce rutiny cmdlet zo vzdialeného napájania Shell:
  
 **Jedného používateľa**
  
Súbor-poštová schránka-identita "Jane Dow"-AuditEnabled $true
  
 **Organizácie**
  
Get-poštová schránka-ResultSize neobmedzené-filter {RecipientTypeDetails-EQ "UserMailbox"} | Súbor schránky-AuditEnabled $true
  
[zistiť viac](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

