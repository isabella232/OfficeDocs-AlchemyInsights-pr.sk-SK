---
title: Prístup služieb dôchodkového
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359378"
---
# <a name="access-services-retirement"></a>Prístup služieb dôchodkového

Ako sme pôvodne oznámená v MC97576, v marci 2017 a naďalej komunikovať v minulom roku prístup služby sú vyňatý z Office 365. Ďalšia fáza v tomto procese bude odstránenie prístupu Web databáz, ktoré používajú zoznamy SharePoint ako ich základný ukladací priestor údajov.

**Ako ma to ovplyvní?**

Od júna 2019, budeme zastaviť vytváranie nových databáz programu Access v službe SharePoint Online a vypnutie služby a všetky zostávajúce aplikácie do apríla roku 2020.

**Čo je potrebné urobiť pre prípravu na túto zmenu?**

Odporúčame vám vytvoriť plán prechodu vaša organizácia prístup web databáz. Správcovia môžete použiť [SharePoint prístup app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) získať súpis prístup aplikácií, ktoré stránky používajú.

Existuje niekoľko spôsobov na migráciu údajov databáz web Access:

- Import do lokálnej databázy Access (. ACCDB) alebo do súboru programu Excel.
- Odporúčame tiež skúmanie Microsoft PowerApps ako alternatívnu platformu vytvoriť bez kódu podnikové riešenia pre web a mobilné zariadenia.