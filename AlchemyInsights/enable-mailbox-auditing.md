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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="cf78a-102">Povoliť auditovanie poštových schránok</span><span class="sxs-lookup"><span data-stu-id="cf78a-102">Enable mailbox auditing</span></span>

<span data-ttu-id="cf78a-103">Ak chcete povoliť auditovanie poštových schránok pre jedného používateľa alebo celú organizáciu, musíte spustiť nasledujúce rutiny cmdlet zo vzdialeného napájania Shell:</span><span class="sxs-lookup"><span data-stu-id="cf78a-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="cf78a-104">**Jedného používateľa**</span><span class="sxs-lookup"><span data-stu-id="cf78a-104">**Single User**</span></span>
  
<span data-ttu-id="cf78a-105">Súbor-poštová schránka-identita "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="cf78a-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="cf78a-106">**Organizácie**</span><span class="sxs-lookup"><span data-stu-id="cf78a-106">**Organization**</span></span>
  
<span data-ttu-id="cf78a-107">Get-poštová schránka-ResultSize neobmedzené-filter {RecipientTypeDetails-EQ "UserMailbox"} | Súbor schránky-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="cf78a-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="cf78a-108">zistiť viac</span><span class="sxs-lookup"><span data-stu-id="cf78a-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

