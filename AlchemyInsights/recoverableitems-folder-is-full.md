---
title: 1336 RecoverableItems priečinok je plný
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741282"
---
# <a name="the-recoverable-items-folder-is-full"></a>Priečinok s využiteľnými položkami je plný

V prípade poštových schránok v službe Exchange Online je predvolený limit ukladacieho priestoru pre priečinok s využiteľnými položkami 30 GB. Limit ukladacieho priestoru pre priečinok s využiteľnými položkami sa automaticky zvýši na 100 GB, ak je poštová schránka umiestnená v zadržaní zadržania, eDiscovery alebo je priradená k politike uchovávania údajov.

Keď priečinok uhraditeľné položky dosiahne limit ukladacieho priestoru, funkčnosť poštovej schránky sa ovplyvní týmito spôsobmi:

- Používateľ nemôže odstrániť položky z poštovej schránky.

- Asistent pre spravované priečinky nedokáže odstrániť položky na základe značiek uchovávania údajov alebo spravovaného priečinka.

- V prípade poštových schránok s možnosťou obnovenia jednej položky, ktoré sú povolené alebo sú podržané, proces ochrany stránky kopírovania a zápisu nemôže zachovať verzie položiek upravovaných používateľom.

- V prípade poštových schránok, ktoré majú zapnuté zapisovanie do denníka auditu poštovej schránky, nie je možné uložiť žiadne položky denníka auditu poštovej schránky do podpriečinka auditov v priečinku uhraditeľné položky.

V prípade poštových schránok, ktoré nie sú zadržané, môžu správcovia použiť `Search-Mailbox -SearchDumpsterOnly -DeleteContent` príkaz v prostredí Exchange Online PowerShell na odstránenie položiek v priečinku uhraditeľné položky. Ďalšie informácie sa nachádzajú v týchto témach:

- [Vyhľadanie a odstránenie správ](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Vyhľadávanie – poštová schránka](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

V prípade poštových schránok, ktoré sú zadržané, musia správcovia pred odstránením položiek z priečinka s využiteľnými položkami odstrániť zadržanie. Ďalšie informácie nájdete v téme [Odstránenie položiek v priečinku uhraditeľné položky v poštových schránkach v cloude zadržaných](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Ak chcete zabrániť tomu, aby sa priečinok uhraditeľné položky stal úplným, správcovia môžu zvýšiť limit ukladacieho priestoru pre priečinok s využiteľnými položkami pre poštové schránky a nastaviť politiku uchovávania poštovej schránky, ktorá premiestni položky z priečinka využiteľné položky do archívnej poštovej schránky používateľa. Pozrite si tému [zvýšenie kvóty uhraditeľných položiek pre poštové schránky v podržaní](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
