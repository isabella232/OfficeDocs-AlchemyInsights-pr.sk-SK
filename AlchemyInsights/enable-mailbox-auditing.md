---
title: Povolenie auditovania poštovej schránky
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: c04f27edc1e22e0e4269758827d5468767967be8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814207"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="2c3b6-102">Povolenie auditovania poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="2c3b6-102">Enable mailbox auditing</span></span>

<span data-ttu-id="2c3b6-103">Ak chcete povoliť auditovanie poštovej schránky pre jedného používateľa alebo pre celú organizáciu, je potrebné spustiť nasledujúce rutiny cmdlet zo vzdialeného prostredia Power Shell:</span><span class="sxs-lookup"><span data-stu-id="2c3b6-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="2c3b6-104">**Jeden používateľ**</span><span class="sxs-lookup"><span data-stu-id="2c3b6-104">**Single User**</span></span>
  
<span data-ttu-id="2c3b6-105">Set-Mailbox identity Jane Dowová – AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="2c3b6-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="2c3b6-106">**Organizácia**</span><span class="sxs-lookup"><span data-stu-id="2c3b6-106">**Organization**</span></span>
  
<span data-ttu-id="2c3b6-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="2c3b6-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="2c3b6-108">zistiť viac</span><span class="sxs-lookup"><span data-stu-id="2c3b6-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

