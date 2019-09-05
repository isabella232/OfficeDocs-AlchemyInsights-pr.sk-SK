---
title: Povoliť auditovanie poštových schránok
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736268"
---
# <a name="enable-mailbox-auditing"></a>Povoliť auditovanie poštových schránok

Ak chcete povoliť auditovanie poštových schránok pre jedného používateľa alebo celú organizáciu, musíte spustiť nasledujúce rutiny cmdlet zo vzdialeného napájania Shell:
  
 **Jedného používateľa**
  
Súbor-poštová schránka-identita "Jane Dow"-AuditEnabled $true
  
 **Organizácie**
  
Get-poštová schránka-ResultSize neobmedzené-filter {RecipientTypeDetails-EQ "UserMailbox"} | Súbor schránky-AuditEnabled $true
  
[zistiť viac](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

