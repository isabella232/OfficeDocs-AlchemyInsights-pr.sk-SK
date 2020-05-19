---
title: Zmena e-mailovej adresy skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283260"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="49736-102">Zmena e-mailovej adresy skupiny Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="49736-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="49736-103">Môžete zmeniť e-mailovú adresu skupiny Microsoft 365 pomocou admin Center.</span><span class="sxs-lookup"><span data-stu-id="49736-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="49736-104">Stačí vybrať skupinu a vybrať @edit e-mailovú adresu.</span><span class="sxs-lookup"><span data-stu-id="49736-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="49736-105">Môžete použiť aj po príkaze EXO PowerShell zmeniť primárnu adresu SMTP skupiny Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="49736-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="49736-106">Súbor UnifiedGroup <Group Name> -primarysmtpaddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="49736-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="49736-107">Príklad:</span><span class="sxs-lookup"><span data-stu-id="49736-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
