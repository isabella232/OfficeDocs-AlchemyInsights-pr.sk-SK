---
title: Po pridaní doplnkov v Outlooku dostane jeden používateľ chybu odmietnutý prístup
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 355f37386e0a498185e195c1d715386785d0b54b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673296"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a>Po pridaní doplnkov v Outlooku dostane jeden používateľ chybu odmietnutý prístup

Používateľské prostredie PowerShell na vyhľadanie povolení:

Get-ManagementRoleAssignment-RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -delegovanie $FALSE | Formát – tabuľka – Automatická rola, RoleAssigneeName, RoleAssigneeType