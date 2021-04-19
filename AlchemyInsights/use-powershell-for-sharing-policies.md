---
title: Používanie prostredia Windows PowerShell na zdieľanie zásad a organizačných vzťahov
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
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826070"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Používanie prostredia Windows PowerShell na zdieľanie zásad a organizačných vzťahov


Pri organizačných vzťahoch si opäť pozrite podrobné informácie o syntaxi a parametroch pre: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  A  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Zásady zdieľania vytvoríte pomocou [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Ak chcete [použiť zásadu zdieľania pre poštovú schránku alebo používateľa](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), musíte použiť kombináciu [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) a [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s novovytvorenou zásadou. Ak chcete [zmeniť, vypnúť alebo odstrániť zásady zdieľania](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), musíte použiť [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) a [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Podrobné informácie o tejto téme nájdete v článku:**

[Zdieľanie v Exchangei Online](https://docs.microsoft.com/exchange/sharing/sharing)