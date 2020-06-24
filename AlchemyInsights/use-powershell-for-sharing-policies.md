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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Používanie prostredia PowerShell na zdieľanie politík a vzťahov organizácie


Pre vzťahy organizácie si prečítajte podrobné informácie o syntaxi a parametri pre : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) a [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Ak chcete vytvoriť politiku zdieľania, použite [novú politiku zdieľania](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Ak chcete [použiť politiku zdieľania pre poštovú schránku alebo používateľa,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) musíte použiť kombináciu [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) a [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s novovytvorenou politikou. Ak chcete [upraviť, vypnúť alebo odstrániť politiku zdieľania,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) musíte použiť [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) a [Odstrániť ZdieľaniePolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Pre úplné pochopenie tejto témy prečítajte si prosím:**

[Zdieľanie v službe Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)