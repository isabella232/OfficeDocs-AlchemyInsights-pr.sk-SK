---
title: Prístup k dôchodkovým službám
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
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698697"
---
# <a name="access-services-retirement"></a>Prístup k dôchodkovým službám

Ako sme boli pôvodne vyhlásené v MC97576, v marci 2017 a pokračovali v komunikácii za uplynulý rok, v ktorom sú služby Accessu v dôchodku. Ďalšou fázou v tomto procese bude odstránenie webových databáz Accessu, ktoré používajú zoznamy SharePointu ako základný ukladací priestor údajov.

**Ako to ovplyvní mňa?**

Od júna 2019 sa ukončí vytváranie nových Accessových databáz v SharePointe Online a vypnutie služby a všetkých zostávajúcich aplikácií do apríla 2020.

**Čo je potrebné urobiť na prípravu tejto zmeny?**

Odporúčame vám vytvoriť plán prechodu pre webové databázy Accessu vašej organizácie. Správcovia môžu použiť [skener aplikácie SharePoint Accessu](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) na získanie zoznamu prístupových aplikácií, ktoré lokality používajú.

Existuje niekoľko spôsobov migrácie údajov webových databáz Accessu:

- Importuje sa do lokálnej Accessovej databázy (. ACCDB) alebo do excelového súboru.
- Odporúčame tiež preskúmať Microsoft PowerApps ako alternatívnu platformu na vytváranie podnikových riešení bez kódu pre webové a mobilné zariadenia.