---
title: 929 doručenú deflectTransport pravidiel
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6cf996e6d0a2698a5ce2bb57251de7c61d248d2a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382680"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="187de-102">Pravidlá pre poštu tok (tiež známy ako pravidlá prenosu)</span><span class="sxs-lookup"><span data-stu-id="187de-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="187de-103">Všeobecný prehľad o mail tok pravidlá: [pravidlá (pravidlá prenosu) v toku pošty](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="187de-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="187de-104">Nastavenie pravidiel pre poštu tok: [pravidlo postupy v toku pošty](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="187de-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="187de-105">Vytvárať, upravovať a mazať pravidlá pre poštu tok: [Správa pošty tok pravidiel](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="187de-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="187de-106">Môžete spravovať pravidlá pre poštu tok v Online PowerShell výmeny.</span><span class="sxs-lookup"><span data-stu-id="187de-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="187de-107">Ďalšie informácie nájdete v časti [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (pohľad), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (vytvoriť), [TransportRule odstrániť](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (zmena existujúceho), [Disable TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (zakázať existujúce), a [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (zapnúť existujúci).</span><span class="sxs-lookup"><span data-stu-id="187de-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="187de-108">Dodatočné mail tok pravidlo cmdlet: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (zoznam dostupných akcií), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (zoznam dostupné podmienky a výnimky), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (pravidlá pre export) a [ Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (Importovať pravidlá).</span><span class="sxs-lookup"><span data-stu-id="187de-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
