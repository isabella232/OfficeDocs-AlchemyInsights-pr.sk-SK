---
title: Automatické šifrovanie niektorých e-mailových správ z balíka Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749457"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatické šifrovanie niektorých e-mailových správ z balíka Office 365

1. V [centre spravovania pre Exchange](https://outlook.office365.com/ecp/)vyberte položku **pravidlá toku pošty >**. 
2. Kliknite na **novú ikonu (+)** a potom kliknite na položku **použiť šifrovanie správ v Office 365 a ochranu práv na správy**.
3. Do poľa **názov** zadajte názov pravidla, napríklad *šifrovať všetky správy*.
4. **Ak chcete použiť toto pravidlo**, vyberte možnosť **[použiť na všetky správy]**. 
5. Vedľa poľa **vykonať** toto políčko kliknite na položku **vybrať jeden**. 
6. V rozbaľovacej ponuke **Šablóna RMS** vyberte položku **šifrovať** a potom kliknite na tlačidlo **OK**. (Ak sa táto možnosť nezobrazuje, znamená to, že váš plán nezahŕňa automatické šifrovanie. Môžete ju však pridať!)
7. Začiarknite políčko **Auditovať Toto pravidlo s úrovňou závažnosti** a potom vyberte požadovanú úroveň. Ak vaša spoločnosť disponuje zmluvnými povinnosťami na odoslanie všetkých zašifrovaných e-mailov, odporúčam nastaviť úroveň na hodnotu **vysoká**.
8. V časti **Vyberte model pre toto pravidlo** kliknite na položku **vynútiť**. 
9. Vyberte ľubovoľný voliteľný výber (zo zoznamu voliteľných výberov, ktoré môžete vykonať v tomto bode, pričom mnohé z nich možno ponechať s predvoleným nastavením pre jednoduchosť).
10. Kliknite na tlačidlo **Uložiť**.

> [!IMPORTANT]
> Vždy sa môžete vrátiť a upraviť toto pravidlo neskôr.

Ďalšie informácie o vytváraní pravidiel šifrovania nájdete v téme [definovanie pravidiel toku pošty na šifrovanie e-mailových správ v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

