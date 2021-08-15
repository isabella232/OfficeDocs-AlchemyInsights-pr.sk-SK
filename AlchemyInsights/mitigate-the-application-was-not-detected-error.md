---
title: Riešenie chyby Aplikácia nebola rozpoznaná
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026129"
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
