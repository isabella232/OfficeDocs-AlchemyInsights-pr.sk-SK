---
title: Zapnutie auditovania poštovej schránky
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429742"
---
# <a name="turn-on-mailbox-auditing"></a><span data-ttu-id="9adb1-102">Zapnutie auditovania poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="9adb1-102">Turn on mailbox auditing</span></span>

<span data-ttu-id="9adb1-103">Ak chcete zapnúť auditovanie poštovej schránky pre jedného používateľa alebo celú organizáciu, spustite nasledujúce rutiny typu cmdlet z vzdialeného prostredia PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9adb1-103">To turn on mailbox auditing for a single user or an entire organization, run the following cmdlets from Remote PowerShell:</span></span>

- <span data-ttu-id="9adb1-104">**Jeden používateľ**: Set-Mailbox identita "Jane Dow" – AuditEnabled $True</span><span class="sxs-lookup"><span data-stu-id="9adb1-104">**Single user**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
- <span data-ttu-id="9adb1-105">**Organizácia**: Get-Mailbox-ResultSize Unlimited-filter {recipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox – AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="9adb1-105">**Organization**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>

<span data-ttu-id="9adb1-106">Ďalšie informácie nájdete v téme [Spravovanie auditovania poštovej schránky](https://go.microsoft.com/fwlink/?linkid=2103668).</span><span class="sxs-lookup"><span data-stu-id="9adb1-106">To learn more, see [Manage mailbox auditing](https://go.microsoft.com/fwlink/?linkid=2103668).</span></span>