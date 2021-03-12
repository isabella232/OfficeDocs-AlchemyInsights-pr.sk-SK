---
title: Automatické šifrovanie niektorých e-mailových správ v Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749444"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatické šifrovanie niektorých e-mailových správ v Office 365

Správy, ktoré používatelia odosielajú určitým externým osobám alebo organizáciám, môžete automaticky šifrovať. Ak to chcete urobiť, vykonajte tieto kroky:

1. V [centre spravovania pre Exchange](https://outlook.office365.com/ecp/)vyberte položku **pravidlá toku pošty >**. 
2. Kliknite na **novú ikonu (+)** a potom kliknite na položku **použiť šifrovanie správ v Office 365 a ochranu práv na správy**.
3. Do poľa **názov** zadajte názov pravidla, napríklad *šifrovanie správ odoslaných do DrToniRamos@gmail.com*.
4. **Ak chcete použiť toto pravidlo**, vyberte položku **príjemca > je touto osobou**. 
5. V okne **Výber členov** vyberte meno osoby, s ktorou chcete použiť pravidlo šifrovania, a potom kliknite na položku **Pridať**. 
6. Po dokončení pridávania používateľov kliknite na tlačidlo **OK**.
7. Vedľa poľa **vykonať** toto políčko kliknite na položku **vybrať jeden**. 
8. V rozbaľovacej ponuke **Šablóna RMS** vyberte položku **šifrovať** a potom kliknite na tlačidlo **OK**. (Ak sa táto možnosť nezobrazuje, znamená to, že váš plán nezahŕňa automatické šifrovanie. Môžete ju však pridať!)
9. Vyberte ľubovoľný voliteľný výber (zo zoznamu voliteľných výberov, ktoré môžete vykonať v tomto bode, pričom mnohé z nich možno ponechať s predvoleným nastavením pre jednoduchosť).
10. Kliknite na tlačidlo **Uložiť**.

> [!IMPORTANT]
> Vždy sa môžete vrátiť a upraviť toto pravidlo neskôr.

Ďalšie informácie o vytváraní pravidiel šifrovania nájdete v téme [definovanie pravidiel toku pošty na šifrovanie e-mailových správ v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

