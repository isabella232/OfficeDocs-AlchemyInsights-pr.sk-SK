---
title: 1336 Priečinok RecoverableItems je plný
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061771"
---
# <a name="the-recoverable-items-folder-is-full"></a>Priečinok Obnoviteľné položky je plný

V Exchange Online poštových schránok je predvolený limit ukladacieho priestoru priečinka Obnoviteľné položky 30 GB. Limit ukladacieho priestoru pre priečinok Obnoviteľné položky sa automaticky zvýši na 100 GB, ak je poštová schránka zadržaná na súdne účely, blokovanie eDiscovery alebo je priradená k politike uchovávania údajov.

Keď sa v priečinku Obnoviteľné položky dosiahne limit ukladacieho priestoru, funkčnosť poštovej schránky sa bude týkať týchto spôsobov:

- Používateľ nemôže odstrániť položky z poštovej schránky.

- Asistent spravovaných priečinkov nemôže odstrániť položky založené na značke uchovávania údajov ani nastaveniach spravovaných priečinkov.

- V prípade poštových schránok, ktoré majú aktivované obnovenie jednej položky alebo sú zadržané, si proces ochrany stránky pri kopírovaní pri písaní nemôže zachovať verzie položiek upravované používateľom.

- V poštových schránkach, v ktorých je zapnuté zapisovanie do denníka auditu poštovej schránky, nie je možné uložiť žiadne položky denníka auditu poštovej schránky v podpriečinku Audity v priečinku Obnoviteľné položky.

V prípade poštových schránok, ktoré nie sú zadržané, môžu správcovia pomocou príkazu v prostredí Exchange Online PowerShell odstrániť položky v priečinku `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Obnoviteľné položky. Ďalšie informácie sa nachádzajú v týchto témach:

- [Vyhľadávanie a odstraňovanie správ](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

V prípade zadržaných poštových schránok musia správcovia odstrániť zadržanie predtým, než budú možné odstránené položky z priečinka Obnoviteľné položky. Ďalšie informácie nájdete v téme [Odstránenie položiek v priečinku Obnoviteľné položky v cloudových poštových schránkach, ktoré sú zadržané.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Správcovia môžu zvýšiť limit ukladacieho priestoru priečinka Obnoviteľné položky pre poštové schránky, čím sa zabráni tomu, aby sa priečinok Obnoviteľné položky zaplnil, a nastaviť politiku uchovávania údajov v poštovej schránke, ktorá premietne položky z priečinka Obnoviteľné položky do archívnej poštovej schránky používateľa. Pozrite [si časť Zvýšenie kvóty Obnoviteľné položky pre zadržané poštové schránky.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
