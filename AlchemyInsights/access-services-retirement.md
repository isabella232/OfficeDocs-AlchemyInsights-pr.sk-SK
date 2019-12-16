---
title: Prístup k službám odchod do dôchodku
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050504"
---
# <a name="access-services-retirement"></a>Prístup k službám odchod do dôchodku

Ako sme pôvodne oznámila v MC97576, v marci 2017, a pokračoval komunikovať za uplynulý rok prístup k službám sú v dôchodku z Office 365. Ďalšou fázou tohto procesu bude odstránenie webových databáz programu Access, ktoré používajú zoznamy lokality SharePoint ako ich základné úložisko údajov.

**Ako to ovplyvní ma?**

Od júna 2019, budeme zastaviť vytváranie nových databáz programu Access v SharePointe Online a vypnúť službu a všetky zostávajúce aplikácie do apríla 2020.

**Čo potrebujem na to, aby ste sa pripravili na túto zmenu?**

Odporúčame vám vytvoriť plán prechodu pre webové databázy programu Access vašej organizácie. Správcovia môžu použiť [skener aplikácie SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) na získanie inventára prístupových aplikácií, ktoré lokality používajú.

Existuje niekoľko spôsobov, ako migrovať údaje webových databáz programu Access:

- Importovanie do lokálnej databázy programu Access (. ACCDB) alebo do súboru programu Excel.
- Odporúčame tiež preskúmať službu Microsoft PowerApps ako alternatívnu platformu na vytvorenie podnikových riešení bez kódu pre webové a mobilné zariadenia.