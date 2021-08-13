---
title: Vyradenie služieb Accessu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938710"
---
# <a name="access-services-retirement"></a>Vyradenie služieb Accessu

Ako sme pôvodne oznámili vo vyhlásení spoločnosti MC97576, v marci 2017, a naďalej komunikovať počas uplynulého roka, Access Services sa pre ich vynechá. Ďalšou fázou tohto procesu bude odstránenie webových databáz Accessu, ktoré používajú SharePoint ako základné ukladanie údajov.

**Ako to na mňa ovplyvní?**

Od júna 2019 zastavíme vytváranie nových accessových databáz v službe SharePoint Online a do apríla 2020 vypneme službu a všetky zostávajúce aplikácie.

**Ako sa mám pripraviť na túto zmenu?**

Odporúčame vám vytvoriť plán prechodu pre webové databázy Accessu vašej organizácie. Správcovia môžu použiť [SharePoint aplikácie Access na](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) získanie inventára aplikácií Accessu, ktoré používajú lokality.

Existuje niekoľko spôsobov migrácie údajov webových databáz Accessu:

- Importovanie do lokálnej databázy Accessu (. ACCDB) alebo na Excel súbor.
- Odporúčame preskúmať Microsoft PowerApps ako alternatívnu platformu, pomocou ktorých môžete vytvoriť podnikové riešenia bez kódu pre web a mobilné zariadenia.