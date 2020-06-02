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
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506969"
---
# <a name="enable-mailbox-auditing"></a>Povoliť auditovanie poštových schránok

Ak chcete povoliť auditovanie poštovej schránky pre jedného používateľa alebo celú organizáciu, z prostredia Remote Power Shell sa musia spustiť nasledujúce rutiny cmdlet:
  
 **Jeden používateľ**
  
Súbor schránky - identita "Jane Dow" -AuditEnabled $true
  
 **Organizácie**
  
Get-Mailbox -ResultSize Neobmedzený -Filter {RecipientTypeDetails-eq "UserMailbox"} | Súbor schránky - AuditEnabled $true
  
[zistiť viac](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

