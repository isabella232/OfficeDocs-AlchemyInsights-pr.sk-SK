---
title: Automatické šifrovanie e-mailových správ v Office 365 odoslaných do určitých domén
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749301"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatické šifrovanie e-mailových správ v Office 365 odoslaných do určitých domén

1. V [centre spravovania pre Exchange](https://outlook.office365.com/ecp/)vyberte položku **pravidlá toku pošty >**. 
2. Kliknite na **novú ikonu (+)** a potom kliknite na položku **použiť šifrovanie správ v Office 365 a ochranu práv na správy**.
3. Do poľa **názov** zadajte názov pravidla, napríklad *šifrovanie správ odoslaných do contoso.com*.
4. **Ak chcete použiť toto pravidlo**, vyberte položku **príjemca > doména**. 
5. Zadajte názov domény, napríklad **contoso.com**.
6. Kliknite na ikonu **Pridať (+)** a potom kliknite na **tlačidlo OK**.
7. Vedľa poľa **vykonať** toto políčko kliknite na položku **vybrať jeden**. 
8. V rozbaľovacej ponuke **Šablóna RMS** vyberte položku **šifrovať** a potom kliknite na tlačidlo **OK**. (Ak sa táto možnosť nezobrazuje, znamená to, že váš plán nezahŕňa automatické šifrovanie. Môžete ju však pridať!)
9. Vyberte ľubovoľný voliteľný výber (zo zoznamu voliteľných výberov, ktoré môžete vykonať v tomto bode, pričom mnohé z nich možno ponechať s predvoleným nastavením pre jednoduchosť).
10. Kliknite na tlačidlo **Uložiť**.

> [!IMPORTANT]
> Vždy sa môžete vrátiť a upraviť toto pravidlo neskôr.

Ďalšie informácie o vytváraní pravidiel šifrovania nájdete v téme [definovanie pravidiel toku pošty na šifrovanie e-mailových správ v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)