---
title: Obísť lobby
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376825"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Ovládanie nastavení vstupnej haly a úrovne účasti

Tieto nastavenia kontrolujú, ktoré účastníci stretnutia čakajú vo vstupnej hale pred tým, ako sú prijatí na schôdzu, a úroveň účasti, ktorú sú povolené na schôdzi. PowerShell môžete použiť na aktualizáciu nastavenia politiky schôdzí, ktoré ešte neboli implementované (označené ako "pripravujeme") v tíme admin Center.  Pozri nižšie pre príklad rutiny cmdlet prostredia PowerShell, ktorá umožňuje všetkým používateľom obísť lobby.  

- [Automaticky priznať](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , že ľudia sú pre-organizátor politiky, ktorá kontroluje, či ľudia pripojiť k schôdzi priamo alebo čakať vo vstupnej hale, kým nie sú prijaté overený používateľ.

- [Umožniť anonymný ľudia začať schôdzu](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je per-organizátor politiky, ktorá kontroluje, či anonymný ľudia, vrátane B2B a federalizovaných používateľov, sa môže pripojiť k schôdzi používateľa bez overený používateľ z organizácie v návštevnosti.

- [Povoliť používateľom telefonického pripojenia k obchádzke lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá kontroluje, či ľudia, ktorí telefonicky pripoja k schôdzi priamo, alebo čakajú vo vstupnej hale bez ohľadu na to, že **automaticky pripúšťajú nastavenie ľudí** .

- [Povoliť organizátorom prepísať nastavenia vstupnej haly](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**pripravujeme**) je politika pre organizátora, ktorá určuje, či organizátor schôdze môže prepísať nastavenia vstupnej haly, ktoré správca nastaví v **automatickom priznávanie osôb** a **povolenie telefonického pripojenia používateľom obísť vstupnú halu** , keď naplánujú novú schôdzu.

**Poznámka:** Prečítajte si článok [spravovanie politík schôdzí v tímoch](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) pre úplný prehľad politík schôdzí spoločnosti Microsoft teams. 


**Príklad PowerShell**

Ak chcete umožniť všetkým, vrátane externých alebo anonymných používateľov, obísť lobby, môžete tiež použiť PowerShell na splnenie tejto úlohy.  Tu je príklad úpravy globálnej politiky schôdzí pre vašu organizáciu.   

(Nezabudnite skontrolovať dokumentáciu vyššie pred vykonaním týchto zmien pochopiť, čo presne to umožňuje.)

Súbor CsTeamsMeetingPolicy-identita globálne-AutoAdmittedUsers "každý"-AllowPSTNUsersToBypassLobby $True

Ďalšie informácie nájdete v téme [súbor CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
