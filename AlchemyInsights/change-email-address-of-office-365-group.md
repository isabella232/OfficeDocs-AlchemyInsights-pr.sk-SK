---
title: Zmena e-mailovej adresy skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819059"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="522c9-102">Zmena e-mailovej adresy skupiny Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="522c9-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="522c9-103">E-mailovú adresu skupiny v Microsoft 365 môžete zmeniť pomocou Centra spravovania.</span><span class="sxs-lookup"><span data-stu-id="522c9-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="522c9-104">Stačí vybrať skupinu a potom položku @upraviť e-mailovú adresu.</span><span class="sxs-lookup"><span data-stu-id="522c9-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="522c9-105">Ak chcete zmeniť primárnu SMTP adresu skupiny Microsoft 365, môžete použiť aj tento príkaz prostredia PowerShell EXO:</span><span class="sxs-lookup"><span data-stu-id="522c9-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="522c9-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="522c9-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="522c9-107">Príklad:</span><span class="sxs-lookup"><span data-stu-id="522c9-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
