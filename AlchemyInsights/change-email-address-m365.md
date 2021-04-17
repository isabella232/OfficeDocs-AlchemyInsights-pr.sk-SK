---
title: Zmena e-mailovej adresy skupiny v Microsoft 365 alebo Microsoft Teams
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819095"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="14ee5-102">Zmena e-mailovej adresy skupiny v Microsoft 365 alebo Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="14ee5-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="14ee5-103">E-mailovú adresu skupiny v Microsoft 365 alebo Microsoft Teams môžete zmeniť pomocou [Centra spravovania služby Microsoft 365](https://admin.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="14ee5-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="14ee5-104">Stačí vybrať skupinu a potom položku @upraviť e-mailovú adresu.</span><span class="sxs-lookup"><span data-stu-id="14ee5-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="14ee5-105">Na zmenu primárnej SMTP adresy skupiny v Microsoft 365 alebo Teams môžete použiť aj nasledujúci príkaz EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="14ee5-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="14ee5-106">Príklad:</span><span class="sxs-lookup"><span data-stu-id="14ee5-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
