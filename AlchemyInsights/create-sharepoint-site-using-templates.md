---
title: Vytvorenie lokality v SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057981"
---
# <a name="create-sharepoint-sites-using-templates"></a>Vytváranie SharePoint lokalít pomocou šablón

Možnosť uložiť lokalitu ako šablónu nie je podporovaná v moderných komunikačných ani tímových lokalitách. Ďalšie informácie o používaní šablón nájdete v téme [Uloženie, stiahnutie a nahratie lokality SharePoint ako šablóny](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Tu je niekoľko bežných problémov alebo riešení týkajúcich sa ukladania lokality alebo zoznamu ako šablóny v SharePointe Online. 

**Tlačidlo Uložiť lokalitu alebo šablónu zoznamu nie je k dispozícii alebo chýba**

Správcovia budú musieť povoliť vlastný skript, aby sa povolili funkcie šablóny. Podrobný postup, príklady a informácie nájdete v téme 

- [Povolenie alebo zakázanie vlastného skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Príkaz Uložiť lokalitu ako šablónu sa nepodporuje a na lokalitách, ktoré používajú infraštruktúru publikovania servera SharePoint Server, môže spôsobiť problémy.

**Šablóna lokality sa nedá vytvoriť alebo nefunguje správne**

V šablóne môže chýbať [funkcia](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a nedá sa aktivovať. Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality na vytvorenie lokality.

- Skontrolujte, či niektoré zo zoznamov alebo knižníc neprekračujú [prahovú veľkosť zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže blokovať vytvorenie šablóny lokality.

- Lokalita môže používať príliš veľa zdrojov, a preto šablóna lokality presahuje limit 50 MB.


- Vyskytujú sa problémy so zobrazovaním údajov zoznamu, ktorý používa vyhľadávací stĺpec. Ďalšie informácie nájdete v téme [V zozname vygenerovanom na základe šablóny sa nezobrazujú údaje zo správneho vyhľadávacieho zoznamu v SharePointe Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Podrobnejšie informácie o bežných problémoch a riešeniach nájdete v téme [Vytvorenie a používanie šablón lokalít.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



