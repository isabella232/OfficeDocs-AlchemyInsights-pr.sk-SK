---
title: Politiky uchovávania údajov v Centre spravovania pre Exchange nefungujú
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952243"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Politiky uchovávania údajov v Centre spravovania pre Exchange

Ak chcete, aby sme spúšťali automatizované kontroly nižšie uvedených nastavení, vyberte tlačidlo Späť < – v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s politikami uchovávania údajov.

Ak máte problémy s politikami uchovávania údajov, ktoré sa v Centre spravovania pre Exchange vzťahujú na poštové schránky a položky, ktoré sa nepresúdnia do archívnej poštovej schránky, skontrolujte toto:

**Koreňové príčiny:**

- **Asistent spravovaných** priečinkov nespracová poštovú schránku používateľa. Asistent spravovaných priečinkov sa pokúsi spracovať každú poštovú schránku vo vašej cloudovej organizácii raz za sedem dní.

  **Riešenie:** Spustite asistenta spravovaných priečinkov.

- **Funkcia RetentionHold** bola **v poštovej** schránke povolená. Ak bola poštová schránka umiestnená na umiestnení lokality RetentionHold, politika uchovávania údajov pre poštovú schránku sa počas tohto času nespracuje.

  **Riešenie:** Skontrolujte stav nastavenia uchovávania údajov a aktualizujte ho podľa potreby. Podrobnosti nájdete v téme Uchovávanie [údajov v poštovej schránke.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Poznámka:** Ak je poštová schránka menšia ako 10 MB, asistent spravovaných priečinkov nebude poštovú schránku automaticky spracovať.
 
Ďalšie informácie o politikách uchovávania údajov v Centre spravovania pre Exchange nájdete v téme:

- [Značky uchovávania údajov a politiky uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Použitie politiky uchovávania údajov pre poštové schránky alebo](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Pridanie alebo odstránenie značiek uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Ako identifikovať typ zadržanej poštovej schránky](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
