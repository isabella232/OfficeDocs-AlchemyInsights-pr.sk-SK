---
title: 929 pravidlá pre doručenú poštu na deflectTransport pravidlá
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724607"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="8a43f-102">Pravidlá toku pošty (známe aj ako pravidlá prenosu)</span><span class="sxs-lookup"><span data-stu-id="8a43f-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="8a43f-103">Všeobecný prehľad pravidiel toku pošty: [pravidlá toku pošty (pravidlá prenosu) v službe Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="8a43f-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="8a43f-104">Nastavenie pravidiel toku pošty: [postupy pravidiel toku pošty v službe Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="8a43f-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="8a43f-105">Vytvorenie, úprava a odstránenie pravidiel toku pošty: [spravovanie pravidiel toku pošty](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="8a43f-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="8a43f-106">Môžete tiež spravovať pravidlá toku pošty v prostredí Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8a43f-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="8a43f-107">Ďalšie informácie nájdete v téme [Get-transporttrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (View), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (vytvoriť), [Remove-Transporttrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (odstrániť), [set-Transporttrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (upraviť existujúce), [zakázať-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (zakázať existujúce), a [Povoliť-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (povoliť existujúce).</span><span class="sxs-lookup"><span data-stu-id="8a43f-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="8a43f-108">Ďalšie rutiny cmdlet pravidlo toku pošty: [Get-Transporttruleaction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (zoznam dostupných akcií), [Get-Transporttrulepredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (zoznam dostupných podmienok a výnimiek), [export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (vývozné pravidlá), a [dovoz-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (dovozné pravidlá).</span><span class="sxs-lookup"><span data-stu-id="8a43f-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
