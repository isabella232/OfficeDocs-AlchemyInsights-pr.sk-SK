---
title: Vytvorenie lokality SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199288"
---
# <a name="create-sharepoint-sites-using-templates"></a>Vytvoriť pomocou šablóny lokality SharePoint

Šablóny lokality SharePoint sú predkompilované definície navrhnuté okolo konkrétnym pracovným požiadavkám. Ďalšie informácie nájdete v téme [pomocou šablóny vytvoriť rôzne typy lokalít SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Tu sú niektoré spoločné problémy/riešenia týkajúce sa uloženia lokality alebo zoznamu ako šablóny lokality Sharepoint online. 

**Uložiť zoznam stránok šablóny tlačidlo nie je k dispozícii alebo chýbajúce**

Správcovia musieť povoliť vlastné skript povoliť funkcie šablóny. Podrobný postup, pozrite si príklady a úvahy 

- [Povolenie alebo zakázanie vlastný skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Uložiť lokalitu ako šablónu príkaz nie je podporovaný a môže spôsobiť problémy na webové stránky používajúce SharePoint Server Publishing infraštruktúry.

**Šablóna lokality sa nedá vytvoriť alebo nefunguje správne**

Šablóna môže byť chýbajúce [funkcie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) a neaktivuje. Ak funkcia nie je k dispozícii na aktiváciu v aktuálnej kolekcii lokalít, nemôžete použiť šablónu lokality vytvoriť lokalitu.

- Skontrolujte, ak žiadne zoznamy alebo knižnice prekročiť [Limit prah zobrazenia zoznamu](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 položiek, pretože to môže zablokovať vytvorenie šablóny lokality.

- Lokality môžu používať príliš veľa zdrojov a preto šablóna lokality prekračuje 50 MB limit.


- Tam sú problémy so zobrazovaním údajov zo zoznamu, ktorý používa vyhľadávacieho stĺpca. Ďalšie informácie nájdete v téme [vytvorené šablóny zoznamu nezobrazuje údaje zo zoznamu správnu vyhľadávania SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Podrobnejšie informácie o spoločné problémy a riešenia, skontrolujte, či [Vytvorenie a používanie šablóny lokality](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



