---
title: Politiky uchovávania údajov v Exchange spravovania nefungujú
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074947"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Politiky uchovávania údajov v Exchange spravovania

Ak chcete, aby sme spúšťali automatizované kontroly nižšie uvedených nastavení, vyberte tlačidlo Späť < – v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s politikami uchovávania údajov.

Ak máte v Centre spravovania pre Exchange problémy s politikami uchovávania údajov, ktoré sa vzťahujú na poštové schránky alebo položky, ktoré sa nepresúdujú do archívnej poštovej schránky, skontrolujte toto:

**Koreňové príčiny:**

- **Asistent spravovaných** priečinkov nespracová poštovú schránku používateľa. Asistent spravovaných priečinkov sa pokúsi spracovať každú poštovú schránku vo vašej cloudovej organizácii raz za sedem dní.

  **Riešenie:** Spustite asistenta spravovaných priečinkov.

- **Funkcia RetentionHold** bola **v poštovej** schránke povolená. Ak bola poštová schránka umiestnená na umiestnení lokality RetentionHold, politika uchovávania údajov pre poštovú schránku sa počas tohto času nespracuje.

  **Riešenie:** Skontrolujte stav nastavenia uchovávania údajov a aktualizujte ho podľa potreby. Podrobnosti nájdete v téme Uchovávanie [údajov v poštovej schránke.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Poznámka:** Ak je poštová schránka menšia ako 10 MB, asistent spravovaných priečinkov nebude poštovú schránku automaticky spracovať.
 
Ďalšie informácie o politikách uchovávania údajov v Exchange spravovania nájdete v týchto téme:

- [Značky uchovávania údajov a politiky uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Použitie politiky uchovávania údajov pre poštové schránky alebo](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Pridanie alebo odstránenie značiek uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Ako identifikovať typ zadržanej poštovej schránky](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
