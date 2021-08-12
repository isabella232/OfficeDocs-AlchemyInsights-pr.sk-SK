---
title: Označenia citlivosti sa nezobrazujú
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061447"
---
# <a name="sensitivity-labels-not-appearing"></a>Označenia citlivosti sa nezobrazujú

Označenia citlivosti umožňujú klasifikáciu a ochranu citlivého obsahu. Možno ich vytvoriť v Centre Centrum dodržiavania súladu pre Microsoft 365, Microsoft 365 zabezpečenia alebo v Centre zabezpečenia & Microsoft 365 v časti Klasifikácia > Označenia citlivosti. Ďalšie informácie o tejto funkcii nájdete [v téme Prehľad označení citlivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Ak ste nakonfigurovali označenia citlivosti, ale v aplikáciách balíka Microsoft 365 sa nezobrazujú, skontrolujte toto:

- Potvrďte, že označenie citlivosti bolo [publikované](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) pre používateľov a skupiny, ktoré chcete.

- Potvrďte, že používateľ používa aplikáciu, ktorá podporuje označenia citlivosti – pozrite [si označenia citlivosti v dokumente.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Ak migrujete [označenia Azure Information Protection,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)uvedomte si dôležité informácie, ktoré sú tu [uvedené.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Podpora ochrany pred stratou údajov (DLP): V súčasnosti sa ako podmienka v politikách DLP môžu použiť iba označenia uchovávania údajov.  Podpora označení citlivosti v politike DLP zatiaľ nie je k dispozícii, ale pracujeme na nej.

- Keď je šifrovanie zapnuté na označení citlivosti, môžete:
    - Priradenie povolení teraz
    - Povolenie používateľom priraďovať povolenia


Ďalšie informácie o možných problémoch nájdete v [téme Známe problémy s označeniami citlivosti.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)