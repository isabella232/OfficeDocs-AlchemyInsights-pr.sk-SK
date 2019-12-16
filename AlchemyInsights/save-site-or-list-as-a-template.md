---
title: Uložiť lokalitu alebo zoznam ako šablónu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048739"
---
# <a name="save-site-or-list-as-a-template"></a>Uložiť lokalitu alebo zoznam ako šablónu

Šablóny lokality SharePoint sú vopred zostavené definície navrhnuté okolo konkrétnej obchodnej potreby. Ďalšie informácie nájdete v téme [Používanie šablón na vytvorenie rôznych typov lokalít SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Tu sú niektoré bežné problémy alebo riešenia týkajúce sa ukladania lokality alebo zoznamu ako šablóny v SharePointe Online.

**Tlačidlo Uložiť šablónu lokality alebo zoznamu nie je k dispozícii alebo chýba**. 

- Správcovia budú musieť povoliť vlastný skript, aby šablóny funkcie. Podrobné kroky, príklady a úvahy nájdete v téme [povolenie alebo zabránenie prispôsobeniu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Príkaz Uložiť lokalitu ako šablónu nie je podporovaný a môže spôsobiť problémy na lokalitách, ktoré používajú SharePoint Server publikovanie infraštruktúry.


**Šablóna lokality sa nedá vytvoriť alebo nepracuje správne**

- Šablóna môže chýbať [funkcia](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a nebude sa aktivovať. Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality na vytvorenie lokality.


- Skontrolujte, či zoznamy alebo knižnice presahujú [limit limitu zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže blokovať vytvorenie šablóny lokality.


- Lokalita môže používať príliš veľa zdrojov, a preto šablóna lokality presahuje limit 50 megabajt (MB).


- Existujú problémy so zobrazením údajov zo zoznamu, ktorý používa vyhľadávací stĺpec. Ďalšie informácie nájdete v časti [zoznam vygenerovaný šablónou nezobrazuje údaje zo správneho vyhľadávacieho zoznamu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Podrobnejšie informácie o bežných problémoch a riešeniach nájdete v referencia, [vytváranie a používanie šablón stránok](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

