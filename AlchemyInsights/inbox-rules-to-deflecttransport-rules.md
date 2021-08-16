---
title: 929 Pravidlá pre doručenú poštu na deflectTransport rules
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
ms.openlocfilehash: a143d36d1656e205311cde4aaff3c0c21815182ee82c60039b2219addac218cb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028667"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>Pravidlá toku pošty (známe aj ako pravidlá prenosu)

- Všeobecný prehľad pravidiel toku pošty: [Pravidlá toku pošty (pravidlá prenosu) v Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)

- Nastavenie pravidiel toku pošty: [Postupy pravidla toku pošty v Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)

- Vytvorenie, úprava a odstránenie pravidiel toku pošty: [Spravovanie pravidiel toku pošty](https://technet.microsoft.com/library/jj657505.aspx)

Pravidlá toku pošty môžete spravovať aj v Exchange Online PowerShell. Ďalšie informácie nájdete v téme [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (zobrazenie), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (vytvoriť), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (odstrániť), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (upraviť existujúce), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (zakázať existujúce) a [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (povoliť existujúce).

Ďalšie rutiny typu cmdlet pravidiel toku pošty: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (zoznam dostupných akcií), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (podmienky a výnimky dostupné v zozname), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (pravidlá exportu) a [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (pravidlá importu).
