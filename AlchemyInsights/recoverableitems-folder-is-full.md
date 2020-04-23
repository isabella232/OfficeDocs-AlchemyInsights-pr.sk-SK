---
title: 1336 RecoverableItems priečinok je plný
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720267"
---
# <a name="the-recoverable-items-folder-is-full"></a>Priečinok Obnoviteľné položky je plný

Pre poštové schránky Exchange Online je predvolený limit ukladacieho priestoru pre priečinok Obnoviteľné položky 30 GB. Limit ukladacieho priestoru pre priečinok Obnoviteľné položky sa automaticky zvýši na 100 GB, ak poštová schránka je umiestnená v zadržanie, eDiscovery hold alebo je priradená politika uchovávania údajov.

Keď priečinok Obnoviteľné položky dosiahne limit ukladacieho priestoru, funkčnosť poštovej schránky je ovplyvnená nasledujúcimi spôsobmi:

- Používateľ nemôže odstrániť položky z poštovej schránky.

- Asistent pre spravované priečinky nemôže odstrániť položky založené na značke uchovávania údajov alebo v nastaveniach spravovaných priečinkov.

- V prípade poštových schránok, ktoré majú povolené obnovenie jednej položky alebo sú umiestnené na podržanie, proces ochrany stránky kopírovania na zápis nemôže zachovať verzie položiek upravených používateľom.

- Pre poštové schránky, ktoré majú schránky auditu zapisovania do denníka zapnutá, žiadne položky denníka auditu poštovej schránky môžu byť uložené v podpriečinku audity v priečinku Obnoviteľné položky.

V prípade poštových schránok, ktoré nie sú podržaných, `Search-Mailbox -SearchDumpsterOnly -DeleteContent` môžu správcovia použiť príkaz v službe Exchange Online PowerShell na odstránenie položiek v priečinku Obnoviteľné položky. Ďalšie informácie sa nachádzajú v týchto témach:

- [Vyhľadávanie a odstraňovanie správ](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

V prípade poštových schránok, ktoré sú podržaný, Správcovia musia odstrániť držanie pred odstránením položiek z priečinka Obnoviteľné položky. Ďalšie informácie nájdete v téme [Odstránenie položiek v priečinku Obnoviteľné položky v poštových schránkach typu cloud na podržanie](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Ak chcete zabrániť úplnému obnoveniu priečinka Obnoviteľné položky, správcovia môžu zvýšiť limit ukladacieho priestoru priečinka Obnoviteľné položky pre poštové schránky zadržaných a nastaviť politiku uchovávania poštových schránok, ktorá presunie položky z priečinka Obnoviteľné položky do archívnej poštovej schránky používateľa. Pozrite si [zvýšenie kvóty pre obnoviteľné položky pre poštové schránky podržaných](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
