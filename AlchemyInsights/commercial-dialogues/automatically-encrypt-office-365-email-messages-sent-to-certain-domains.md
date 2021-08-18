---
title: Automatické šifrovanie Office 365 e-mailových správ odoslaných do určitých domén
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318863"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatické šifrovanie Office 365 e-mailových správ odoslaných do určitých domén

1. V Centre [spravovania Exchange vyberte](https://outlook.office365.com/ecp/)položku **Pravidlá toku > pošty**. 
2. Kliknite na **ikonu Nové (+)** a potom kliknite na **položku Šifrovanie správ v Office 365 a ochranu práva na správy**.
3. Do **poľa** Názov zadajte názov pravidla, napríklad Šifrovať správy *odoslané* contoso.com .
4. V **časti Použiť toto pravidlo ak** vyberte položku Príjemca > **je**. 
5. Zadajte názov domény, napríklad **contoso.com.**
6. Kliknite na **ikonu Pridať (+)** a potom kliknite na tlačidlo **OK.**
7. Vedľa poľa **Vykonajte nasledovné kliknite** na položku **Vybrať.** 
8. V **rozbaľovacej ponuke šablóny RMS** vyberte položku **Zašifrovať a** potom kliknite na tlačidlo **OK.** (Ak sa táto možnosť zobraziť, znamená to, že váš plán nezahŕňa automatické šifrovanie. Môžete ho však pridať!)
9. Vyberte ľubovoľnú voliteľnú možnosť (zo zoznamu voliteľných výberov, ktoré môžete v tomto momente vybrať, z ktorých mnohé môžete ponechať s predvoleným nastavením jednoduchosti).
10. Kliknite na tlačidlo **Uložiť**.

**Dôležité:** Toto pravidlo môžete vždy vrátiť a upraviť neskôr.

Ďalšie informácie o vytváraní pravidiel šifrovania nájdete v téme Definovanie pravidiel toku pošty na [šifrovanie e-mailových správ vo Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)