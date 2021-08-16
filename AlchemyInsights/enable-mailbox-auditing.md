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
ms.openlocfilehash: 176fdc57c6453cafe6ca773d845f8f59ea782089e3e33ad70909ed495aa1a8c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003035"
---
# <a name="enable-mailbox-auditing"></a>Povolenie auditovania poštovej schránky

Ak chcete povoliť auditovanie poštovej schránky pre jedného používateľa alebo pre celú organizáciu, je potrebné spustiť nasledujúce rutiny cmdlet zo vzdialeného prostredia Power Shell:
  
 **Jeden používateľ**
  
Set-Mailbox identity Jane Dowová – AuditEnabled $true
  
 **Organizácia**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[Ďalšie informácie](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

