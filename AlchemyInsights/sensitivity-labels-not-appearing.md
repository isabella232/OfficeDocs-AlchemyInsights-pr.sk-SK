---
title: Označenia citlivosti sa nezobrazujú
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 1326eca02044014a8e9c072fcc3e4cd3a41c7a9f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511667"
---
# <a name="sensitivity-labels-not-appearing"></a>Označenia citlivosti sa nezobrazujú

Označenia citlivosti umožňujú klasifikáciu a ochranu citlivého obsahu. Môžu byť vytvorené v Centre súladu s požiadavkami služby Microsoft 365, Centrum zabezpečenia spoločnosti Microsoft 365 alebo Centrum zabezpečenia spoločnosti Microsoft 365 & centrum súladu v časti Menovky klasifikácie > citlivosti. Ďalšie informácie o tejto funkcii nájdete v téme [Prehľad menoviek citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Ak ste nakonfigurovali menovky citlivosti, ale nezobrazujú sa v aplikáciách balíka Office, skontrolujte nasledovné:

- Potvrďte, že označenie citlivosti bolo [publikované](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) požadovaným používateľom a skupinám.

- Skontrolujte, či používateľ používa aplikáciu, ktorá podporuje označenia citlivosti - pozrite si [označenia citlivosti v dokumente](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Ak [migrujete štítky Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)uvedomte si tu [uvedené](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)úvahy .

- Podpora ochrany pred únikom údajov (DLP): V súčasnosti možno ako podmienku v politikách DLP použiť iba štítky uchovávania údajov.  Podpora označení citlivosti v politike DLP ešte nie je k dispozícii, ale pracujeme na tom.

- Ak je šifrovanie zapnuté na štítku citlivosti, môžete vybrať možnosť:
    - Priradenie povolení
    - Umožniť používateľom priradiť povolenia


Ďalšie informácie o možných problémoch nájdete v téme [Známe problémy s označeniami citlivosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).