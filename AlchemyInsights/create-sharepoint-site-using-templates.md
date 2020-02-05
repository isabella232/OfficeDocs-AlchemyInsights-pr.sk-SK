---
title: Vytvorenie lokality SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770438"
---
# <a name="create-sharepoint-sites-using-templates"></a>Vytvorenie lokalít SharePoint pomocou šablón

Možnosť uloženia stránky ako šablóny nie je podporovaná modernými komunikačnými alebo tímových lokalít. Ďalšie informácie o používaní šablón nájdete [v téme Uloženie, prevzatie a odovzdanie lokality SharePoint ako šablóny](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Tu sú niektoré bežné problémy alebo riešenia týkajúce sa ukladania lokality alebo zoznamu ako šablóny v SharePointe Online. 

**Tlačidlo Uložiť stránku alebo šablónu zoznamu nie je k dispozícii alebo chýba**

Správcovia budú musieť povoliť vlastný skript, aby šablóny funkcie. Podrobné kroky, príklady a úvahy nájdete v časti 

- [Povolenie alebo zabránenie prispôsobeniu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Príkaz Uložiť lokalitu ako šablónu nie je podporovaný a môže spôsobiť problémy na lokalitách, ktoré používajú SharePoint Server publikovanie infraštruktúry.

**Šablóna lokality sa nedá vytvoriť alebo nepracuje správne**

Šablóna môže chýbať [funkcia](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a nebude sa aktivovať. Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality na vytvorenie lokality.

- Skontrolujte, či zoznamy alebo knižnice presahujú [limit limitu zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže blokovať vytvorenie šablóny lokality.

- Lokalita môže používať príliš veľa zdrojov, a preto šablóna lokality presahuje limit 50 MB.


- Existujú problémy so zobrazením údajov zo zoznamu, ktorý používa vyhľadávací stĺpec. Ďalšie informácie nájdete v časti [zoznam vygenerovaný šablónou nezobrazuje údaje zo správneho vyhľadávacieho zoznamu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Podrobnejšie informácie o bežných problémoch a riešeniach nájdete v téme [Vytvorenie a používanie šablón lokality](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



