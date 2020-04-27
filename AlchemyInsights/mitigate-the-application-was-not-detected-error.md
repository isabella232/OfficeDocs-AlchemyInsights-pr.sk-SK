---
title: Riešenie chyby Aplikácia nebola rozpoznaná
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810498"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Riešenie chyby Aplikácia nebola rozpoznaná

Chyba inštalácie aplikácie „Aplikácia nebola rozpoznaná po úspešnom dokončení inštalácie“ nahlásená službou Intune sa môže vyskytnúť vo všetkých hlavných platformách operačného systému (Windows, iOS a Android).

Najbežnejšie scenáre, pri ktorých sa vyskytne táto chyba, zahŕňajú:

- Aplikácia bola aktualizovaná mimo služby Intune (z obchodu s aplikáciami tretej strany) po počiatočnom nasadení. Príklad: Niektoré aplikácie, napríklad Google Chrome, môžu vykonávať automatické aktualizácie.
- Používateľ odinštaloval aplikáciu po počiatočnej inštalácii.

Ak chcete vyriešiť tento problém, najskôr skontrolujte ovplyvnené zariadenia a zistite, v ktorom scenári sa chyba vyskytuje.

- Ak bola aplikácia aktualizovaná mimo služby Intune, nasadenie aplikácie je možné nastaviť na ignorovanie verzie aplikácie. Ak to chcete urobiť, v časti **Konfigurácia aplikácie > Informácie o aplikácii** nastavte položku **Ignorovaťnú verziu aplikácie** na možnosť **Áno**.
- Pri zacielení na klienta môže byť vhodné nasadiť aplikáciu ako „povinnú“ a zabezpečiť, aby sa nasadila najnovšia verzia.
- Prípadne na platforme iOS je možné použiť funkciu **automatickej aktualizácie** spojenej s programom Apple Volume Purchase Program, ktorú je možné nakonfigurovať tak, aby automaticky aktualizovala na nové verzie aplikácií, keď budú k dispozícii.

Ďalšie informácie o riešení problémov s inštaláciou aplikácií nájdete v téme [Riešenie problémov s inštaláciou aplikácií](https://docs.microsoft.com/intune/troubleshoot-app-install).
