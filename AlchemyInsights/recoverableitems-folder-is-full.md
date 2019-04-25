---
title: 1336 RecoverableItems priečinok je plný.
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389098"
---
# <a name="the-recoverable-items-folder-is-full"></a>Priečinok Obnoviteľné položky je plný

Schránky Exchange Online v Office 365, predvolené ukladacieho priečinka Obnoviteľné položky je 30 GB. Ukladacieho priečinka Obnoviteľné položky sa automaticky zvýši na 100 GB, ak poštová schránka je umiestnený na zadržanie, podržte eDiscovery, alebo je priradená k politike uchovávania údajov služby Office 365.

Keď priečinka Obnoviteľné položky dosiahne limit ukladacieho priestoru, schránky funkčnosť je ovplyvnený nasledovnými spôsobmi:

- Používateľa nemôžete odstrániť položky z poštovej schránky.

- Asistent pre spravované priečinky nemožno odstrániť položky založené na značku uchovávania údajov alebo spravovaných priečinkov nastavenia.

- Pre poštové schránky, ktoré majú jediný obnovenie položky zapnuté alebo sa odloží, procese ochrany kópiu na zápis stránky nemôže zachovať verzie položiek upravil používateľ.

- Pre poštové schránky, ktoré majú zapnuté zapisovanie auditu poštovej schránky, žiadne položky denníka auditu poštovej schránky môžu byť uložené v podpriečinku auditov v priečinku Obnoviteľné položky.

Pre poštové schránky, ktoré nie sú zadržané, správcovia môžu použiť `Search-Mailbox -SearchDumpsterOnly -DeleteContent` príkaz Exchange Online PowerShell odstrániť položky v priečinku Obnoviteľné položky. Ďalšie informácie sa nachádzajú v týchto témach: 

- [Vyhľadanie a odstránenie správ](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Pre poštové schránky, ktoré sú podržané, správcovia majú odstrániť hold, ako budú môcť odstránené položky z priečinka Obnoviteľné položky. Ďalšie informácie nájdete v téme [odstrániť položky Obnoviteľné položky priečinka poštovými schránkami na držať](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Zabrániť stáva plne priečinka Obnoviteľné položky, správcovia môžu zvýšiť limit pre skladovanie Obnoviteľné položky priečinka poštové schránky na držať a nastaviť politiku uchovávania údajov poštovej schránky, ktoré premiestni položky z priečinka Obnoviteľné položky používateľa Archív Poštová schránka. Vidieť [zvýšenie Obnoviteľné položky kvóty poštových schránok na hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
