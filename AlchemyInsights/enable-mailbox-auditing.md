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
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="0e310-102">Povoliť auditovanie poštových schránok</span><span class="sxs-lookup"><span data-stu-id="0e310-102">Enable mailbox auditing</span></span>

<span data-ttu-id="0e310-103">Ak chcete povoliť auditovanie poštových schránok pre jedného používateľa alebo celú organizáciu, musíte spustiť nasledujúce rutiny cmdlet zo vzdialeného napájania Shell:</span><span class="sxs-lookup"><span data-stu-id="0e310-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="0e310-104">**Jedného používateľa**</span><span class="sxs-lookup"><span data-stu-id="0e310-104">**Single User**</span></span>
  
<span data-ttu-id="0e310-105">Súbor-poštová schránka-identita "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="0e310-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="0e310-106">**Organizácie**</span><span class="sxs-lookup"><span data-stu-id="0e310-106">**Organization**</span></span>
  
<span data-ttu-id="0e310-107">Get-poštová schránka-ResultSize neobmedzené-filter {RecipientTypeDetails-EQ "UserMailbox"} | Súbor schránky-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="0e310-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="0e310-108">zistiť viac</span><span class="sxs-lookup"><span data-stu-id="0e310-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

