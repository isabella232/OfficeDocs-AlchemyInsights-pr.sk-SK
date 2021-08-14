---
title: Automatické šifrovanie určitých e Office 365-mailových správ
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
ms.openlocfilehash: 8ae1c6853f41790efc3b24a9dc696bccf8385967d8c9219a1200e287e6ce32a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53949582"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatické šifrovanie určitých e Office 365-mailových správ

Správy, ktoré používatelia odosielajú určitým externým ľuďom alebo organizáciám, môžete automaticky šifrovať. Vykonáte to vykonaním týchto krokov:

1. V Centre [Exchange vyberte](https://outlook.office365.com/ecp/)položku **Tok pošty a > správ**. 
2. Kliknite na **ikonu Nové (+)** a potom kliknite na **položku Šifrovanie správ v Office 365 a ochranu prístupových práv na správy**.
3. Do **poľa** Názov zadajte názov pravidla, napríklad Šifrovať správy *odoslané DrToniRamos@gmail.com*.
4. V **časti Použiť toto pravidlo ak** vyberte položku Príjemca > je táto **osoba**. 
5. V okne **Výber členov** vyberte meno osoby, pre ktorú chcete použiť pravidlo šifrovania, a potom kliknite na položku **Pridať**. 
6. Po pridaní používateľov kliknite na tlačidlo **OK.**
7. Vedľa poľa **Vykonajte nasledovné kliknite** na položku **Vybrať.** 
8. V **rozbaľovacej ponuke šablóny RMS** vyberte položku **Zašifrovať a** potom kliknite na tlačidlo **OK.** (Ak sa táto možnosť zobraziť, znamená to, že váš plán nezahŕňa automatické šifrovanie. Môžete ho však pridať!)
9. Vyberte ľubovoľnú voliteľnú možnosť (zo zoznamu voliteľných výberov, ktoré môžete v tomto momente vybrať, z ktorých mnohé môžete ponechať s predvoleným nastavením jednoduchosti).
10. Kliknite na tlačidlo **Uložiť**.

> [!IMPORTANT]
> Toto pravidlo sa vždy môžete vrátiť a toto pravidlo upraviť neskôr.

Ďalšie informácie o vytváraní pravidiel šifrovania nájdete v téme Definovanie pravidiel toku pošty na [šifrovanie e-mailových správ vo Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

