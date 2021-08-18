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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324005"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Riešenie bežných problémov s formátovaním záznamov DKIM

Väčšina problémov s nastavením DKIM súvisí s nesprávnymi DNS záznamami.

Ak chcete vyriešiť problémy s nastavením DKIM, overte, či je CNAME záznam DKIM **(nie** TXT záznam) naformátovaný správne. Ďalšie informácie nájdete v téme Čo je potrebné urobiť na manuálne nastavenie [DKIM v Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Ak potrebujete pomoc so záznamami DNS vo všeobecnosti, pozrite si [tému Vytvorenie DNS záznamov u ľubovoľného](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)poskytovateľa hostiteľských služieb DNS pre Office 365 .

**Poznámka:** Po vytvorení alebo aktualizácii DNS záznamov DKIM v hostiteľskej službe DNS pre vašu doménu budete musieť počkať, kým sa DNS záznamy budú šíriť.
