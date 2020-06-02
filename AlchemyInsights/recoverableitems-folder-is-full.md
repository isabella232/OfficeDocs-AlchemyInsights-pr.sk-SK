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
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510767"
---
# <a name="the-recoverable-items-folder-is-full"></a>Priečinok Obnoviteľné položky je plný

Pre poštové schránky služby Exchange Online je predvolený limit ukladacieho priestoru pre priečinok Obnoviteľné položky 30 GB. Limit ukladacieho priestoru pre priečinok Obnoviteľné položky sa automaticky zvýši na 100 GB, ak je poštová schránka umiestnená v zadržaní v dôsledku súdneho sporu, zadržaní elektronického vyhľadávania alebo priradená k politike uchovávania údajov.

Keď priečinok Obnoviteľné položky dosiahne limit ukladacieho priestoru, funkcie poštovej schránky je ovplyvnená nasledujúcimi spôsobmi:

- Používateľ nemôže odstrániť položky z poštovej schránky.

- Asistent pre spravované priečinky nemôže odstrániť položky na základe značky uchovávania údajov alebo nastavenia spravovaného priečinka.

- Pre poštové schránky, ktoré majú jeden bod obnovenia zapnuté alebo sú umiestnené pouložené, proces ochrany stránky copy-on-write nemôže zachovať verzie položiek upravovaných používateľom.

- Pre poštové schránky, ktoré majú poštovej schránky auditu zapisovania do denníka zapnuté, žiadne položky denníka auditu poštovej schránky môžu byť uložené v podpriečinku Audity v priečinku Obnoviteľné položky.

Pre poštové schránky, ktoré nie sú zadržané, správcovia môžu použiť `Search-Mailbox -SearchDumpsterOnly -DeleteContent` príkaz v prostredí Exchange Online PowerShell na odstránenie položiek v priečinku Obnoviteľné položky. Ďalšie informácie sa nachádzajú v týchto témach:

- [Vyhľadávanie a odstraňovanie správ](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Poštová schránka vyhľadávania](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

V prípade poštových schránok, ktoré sú zadržané, správcovia musia odstrániť zadržanie pred odstránením položiek z priečinka Obnoviteľné položky. Ďalšie informácie sa nachádzajú v téme [Odstránenie položiek v priečinku Obnoviteľné položky poštových schránok typu cloud v zadržaných poštových schránkach typu cloud](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

S cieľom zabrániť tomu, aby sa priečinok Obnoviteľné položky nestal plným, správcovia môžu zvýšiť limit ukladacieho priestoru priečinka Obnoviteľné položky pre poštové schránky zadržané a nastaviť politiku uchovávania údajov poštovej schránky, ktorá presunie položky z priečinka Obnoviteľné položky do archívnej poštovej schránky používateľa. Ďalšie informácie nájdete v téme [Zvýšenie kvóty Obnoviteľné položky pre poštové schránky v zadržaných poštových schránkach](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
