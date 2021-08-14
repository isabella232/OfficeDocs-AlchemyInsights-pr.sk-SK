---
title: Riešenie bežných problémov s formátovaním záznamov DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930076"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Riešenie bežných problémov s formátovaním záznamov DKIM

Väčšina problémov s nastavením DKIM súvisí s nesprávnymi DNS záznamami.

Ak chcete vyriešiť problémy s nastavením DKIM, overte, či je CNAME záznam DKIM **(nie** TXT záznam) naformátovaný správne. Ďalšie informácie nájdete v téme Čo je potrebné urobiť na manuálne nastavenie [DKIM v Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Ak potrebujete pomoc so záznamami DNS vo všeobecnosti, pozrite si tému Vytvorenie DNS záznamov [u ľubovoľného](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)poskytovateľa hostiteľských služieb DNS pre Office 365 .

> [!NOTE]
> Po vytvorení alebo aktualizácii DNS záznamov DKIM v hostiteľskej službe DNS pre vašu doménu budete musieť počkať, kým sa DNS záznamy budú šíriť.
