---
title: pravidlá pre doručenú poštu v 929 na deflectTransport pravidlá
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: abb729c40fb87bcca8cc03c95aa4677597d20c08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778706"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="bf62a-102">Pravidlá toku pošty (známe aj ako pravidlá prenosu)</span><span class="sxs-lookup"><span data-stu-id="bf62a-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="bf62a-103">Všeobecný prehľad pravidiel toku pošty: [pravidlá toku pošty (pravidlá prenosu) v službe Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="bf62a-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="bf62a-104">Nastavenie pravidiel toku pošty: [postupy pravidiel toku pošty v službe Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="bf62a-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="bf62a-105">Vytvorenie, úprava a odstránenie pravidiel toku pošty: [spravovanie pravidiel toku pošty](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="bf62a-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="bf62a-106">Pravidlá toku pošty tiež môžete spravovať v prostredí Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bf62a-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="bf62a-107">Ďalšie informácie nájdete v téme [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (Zobraziť), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (Create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (Delete), [set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (upraviť existujúce), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (zakázať existujúce) a [Povoliť-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (povoliť existujúce).</span><span class="sxs-lookup"><span data-stu-id="bf62a-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="bf62a-108">Ďalšie rutiny cmdlet pravidiel toku pošty: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (zoznam dostupných akcií), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (zoznam dostupných podmienok a výnimiek), [export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (exportné pravidlá) a [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (dovozné pravidlá).</span><span class="sxs-lookup"><span data-stu-id="bf62a-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
