---
title: Uloženie lokality alebo zoznamu ako šablóny
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727546"
---
# <a name="save-site-or-list-as-a-template"></a>Uloženie lokality alebo zoznamu ako šablóny

Šablóny lokality SharePoint sú vopred definované definície navrhnuté okolo konkrétnej podnikovej potreby. Ďalšie informácie nájdete v téme [Používanie šablón na vytvorenie rôznych druhov lokalít SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Tu je niekoľko bežných problémov a riešení, ktoré sa týkajú ukladania lokality alebo zoznamu ako šablóny v SharePointe Online.

**Tlačidlo Uložiť šablónu lokality alebo zoznamu nie je k dispozícii alebo chýba**. 

- Správcovia budú musieť povoliť vlastné skripty na povolenie funkcií šablón. Podrobné kroky, príklady a poznámky nájdete v téme [povolenie alebo zakázanie vlastného skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Príkaz Uložiť lokalitu ako šablónu nie je podporovaný a môže spôsobovať problémy na lokalitách, v ktorých sa používa Infraštruktúra publikovania servera SharePoint Server.


**Šablónu lokality nie je možné vytvoriť alebo nefunguje správne**

- Šablóna môže chýbať [funkcia](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a nedá sa aktivovať. Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality na vytvorenie lokality.


- Skontrolujte, či niektoré zoznamy alebo knižnice presiahnu [limitné hodnoty zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže blokovať vytvorenie šablóny lokality.


- Lokalita môže používať príliš veľa zdrojov, a preto šablóna lokality prekračuje limit 50 megabajtov (MB).


- Vyskytli sa problémy so zobrazením údajov zo zoznamu, ktorý používa vyhľadávací stĺpec. Ďalšie informácie nájdete v téme [zoznam generovaný šablónou sa nezobrazujú údaje zo správneho vyhľadávacieho zoznamu v SharePointe Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Podrobnejšie informácie o bežných problémoch a riešeniach nájdete v odkaze na [Vytvorenie a použitie šablón lokalít](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

