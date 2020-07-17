---
title: Používanie prostredia PowerShell na zdieľanie politík a vzťahov organizácie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862155"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="494dc-102">Používanie prostredia PowerShell na zdieľanie politík a vzťahov organizácie</span><span class="sxs-lookup"><span data-stu-id="494dc-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="494dc-103">Pre vzťahy organizácie si prečítajte podrobné informácie o syntaxi a parametri pre : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) a [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="494dc-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="494dc-104">Ak chcete vytvoriť politiku zdieľania, použite [novú politiku zdieľania](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="494dc-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="494dc-105">Ak chcete [použiť politiku zdieľania pre poštovú schránku alebo používateľa,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) musíte použiť kombináciu [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) a [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s novovytvorenou politikou.</span><span class="sxs-lookup"><span data-stu-id="494dc-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="494dc-106">Ak chcete [upraviť, vypnúť alebo odstrániť politiku zdieľania,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) musíte použiť [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) a [Odstrániť ZdieľaniePolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="494dc-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="494dc-107">**Pre úplné pochopenie tejto témy prečítajte si prosím:**</span><span class="sxs-lookup"><span data-stu-id="494dc-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="494dc-108">Zdieľanie v službe Exchange Online</span><span class="sxs-lookup"><span data-stu-id="494dc-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)