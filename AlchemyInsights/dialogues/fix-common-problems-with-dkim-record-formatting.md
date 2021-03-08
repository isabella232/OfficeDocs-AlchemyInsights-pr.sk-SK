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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525646"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Riešenie bežných problémov s formátovaním záznamov DKIM

Väčšinu problémov s nastavením DKIM súvisia s nesprávnymi záznamami DNS.

Ak chcete vyriešiť problémy s nastavením DKIM, overte, či je záznam CNAME CNAME (**nie** txt záznam) naformátovaný správne. Ďalšie informácie nájdete v téme [čo je potrebné urobiť na manuálne nastavenie funkcie dkim v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Ak potrebujete pomoc so záznamami DNS všeobecne, pozrite si tému [Vytvorenie záznamov DNS u ktoréhokoľvek poskytovateľa hostiteľských služieb DNS pre Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> Po vytvorení alebo aktualizácii DNS záznamov v hostiteľskej službe DNS pre svoju doménu budete musieť počkať na propagáciu DNS záznamov.
