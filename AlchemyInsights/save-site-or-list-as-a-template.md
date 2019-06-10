---
title: Uložiť ako šablónu lokality alebo zoznamu
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 73a32536995a604c734393c2300b4c9bb507e2b2
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770542"
---
# <a name="save-site-or-list-as-a-template"></a>Uložiť ako šablónu lokality alebo zoznamu

Šablóny lokality SharePoint sú predkompilované definície navrhnuté okolo konkrétnym pracovným požiadavkám. Ďalšie informácie nájdete v téme [pomocou šablóny vytvoriť rôzne typy lokalít SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Tu sú niektoré spoločné problémy/riešenia týkajúce sa uloženia lokality alebo zoznamu ako šablóny lokality SharePoint Online.

**Uložiť zoznam stránok šablóny tlačidlo je nie sú k dispozícii alebo chýbajúce**. 

- Správcovia musieť povoliť vlastné skript povoliť funkcie šablóny. Podrobný postup, príklady a úvah nájdete [Povoliť alebo zakázať vlastný skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Uložiť lokalitu ako šablónu príkaz nie je podporovaný a môže spôsobiť problémy na webové stránky používajúce SharePoint Server Publishing infraštruktúry.


**Šablóna lokality sa nedá vytvoriť alebo nefunguje správne**

- Šablóna môže byť chýbajúce [funkcie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a neaktivuje. Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality vytvoriť lokalitu.


- Skontrolujte, ak žiadne zoznamy alebo knižnice prekročiť [Limit prah zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže zablokovať vytvorenie šablóny lokality.


- Lokality môžu používať príliš veľa prostriedkov a preto šablóna lokality presahuje limit 50 megabajtov (MB).


- Tam sú problémy so zobrazovaním údajov zo zoznamu, ktorý používa vyhľadávacieho stĺpca. Ďalšie informácie nájdete v téme [vytvorené šablóny zoznamu nezobrazuje údaje zo zoznamu správnu vyhľadávania SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


Pre podrobnejšie informácie o spoločných problémoch a riešeniach prosím odkaz, [Vytvorenie a používanie šablóny lokality](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

