---
title: Umiestnenie údajov
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655297"
---
# <a name="data-location"></a>Umiestnenie údajov

Môžete zobraziť umiestnenie nájomcu v admin Center alebo pripojením na Exchange Online cez PowerShell.


**Admin Center:**
1. Prihláste sa do [centra spravovania](https://admin.microsoft.com/Adminportal/Home).
2. Vyberte položku **Nastavenie** > **profilu organizácie**.
3. V časti **Umiestnenie údajov**vyberte položku **Zobraziť podrobnosti**.


**Powershell:**
1. Pripojenie k službe Exchange Online pomocou prostredia Windows PowerShell.
2. Spustiť rutiny cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) Zobraziť zoznam vlastností nájomcu. 
3. Pozrite sa na vlastnosť OrganizationId.

Ak máte umiestnenie údajov pre EXO a SPO, môžete určiť umiestnenie údajov pre iné služby, ktoré môžete použiť z [miesta, kde sa vaše údaje nachádzajú](https://products.office.com/where-is-your-data-located).