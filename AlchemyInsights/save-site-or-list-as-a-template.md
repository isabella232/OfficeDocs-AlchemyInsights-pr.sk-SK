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
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109219"
---
# <a name="save-site-or-list-as-a-template"></a>Uloženie lokality alebo zoznamu ako šablóny

SharePoint šablóny lokalít sú vopred vytvorené definície navrhnuté na základe konkrétnych pracovných potreby. Ďalšie informácie nájdete v téme [Používanie šablón na vytvorenie rôznych druhov SharePoint lokalít.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Tu je niekoľko bežných problémov alebo riešení týkajúcich sa ukladania lokality alebo zoznamu ako šablóny vo SharePoint Online.

**Tlačidlo Uložiť šablónu lokality alebo zoznamu nie je k dispozícii alebo chýba.** 

- Správcovia budú musieť povoliť vlastný skript, aby sa povolili funkcie šablóny. Podrobné kroky, príklady a informácie nájdete v téme Povolenie [alebo zabránenie vlastného skriptu.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Príkaz Uložiť lokalitu ako šablónu sa nepodporuje a na lokalitách, ktoré používajú infraštruktúru publikovania servera SharePoint Server, môže spôsobiť problémy.


**Šablóna lokality sa nedá vytvoriť alebo nefunguje správne**

- V šablóne môže chýbať [funkcia](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a nedá sa aktivovať. Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality na vytvorenie lokality.


- Skontrolujte, či niektoré zo zoznamov alebo knižníc neprekračujú [prahovú veľkosť zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže blokovať vytvorenie šablóny lokality.


- Lokalita pravdepodobne používa príliš veľa prostriedkov, šablóna lokality preto presahuje limit 50 megabajtov (MB).


- Vyskytujú sa problémy so zobrazovaním údajov zoznamu, ktorý používa vyhľadávací stĺpec. Ďalšie informácie nájdete v téme V zozname vygenerovanej na základe šablóny sa údaje zo [správneho vyhľadávacieho zoznamu v SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Podrobnejšie informácie o bežných problémoch a riešeniach nájdete v téme [Vytvorenie a používanie šablón lokalít.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

