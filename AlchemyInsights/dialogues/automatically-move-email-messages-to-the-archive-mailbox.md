---
title: Automatické presúvanie e-mailových správ do archívnej poštovej schránky
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527100"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatické presúvanie e-mailových správ do archívnej poštovej schránky

Tu je postup, ako nastaviť politiku na automatické premiestnenie starého e-mailu používateľa do archívnej poštovej schránky:

1. Prejdite na položky [**zabezpečenie & súladu s predpismi**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  na **správu údajov**  >   a overte, či je pre používateľa povolená archivácia poštovej schránky. Ak nie, kliknite na položku **Povoliť** a potom v poli upozornenie na tlačidlo **Áno** .
2. Prejdite do centra spravovania pre [**Exchange > spravovanie súladu > značky uchovávania údajov**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Vyberte ikonu + a potom vyberte položku **automaticky použiť na celú poštovú schránku**.
4. Priraďte názov značky uchovávania údajov a vyberte položku **premiestniť do archívu**. Pre obdobie uchovávania údajov zadajte požadovaný čas, napríklad 90 dní. Kliknite na tlačidlo **Uložiť**.
5. Teraz vytvorte politiku uchovávania údajov: vyberte položku **politiky uchovávania údajov**, vyberte ikonu, ak chcete pridať novú politiku.
6. Priraďte názov k politike uchovávania údajov, potom kliknutím a posunutím vyhľadajte a pridajte značku uchovávania údajov, ktorú ste práve vytvorili. Kliknite na tlačidlo **Uložiť**.
7. Nakoniec použite politiku uchovávania údajov v poštovej schránke používateľa: stále v centre spravovania pre Exchange prejdite na položku  >  **poštové schránky** príjemcov. Vyberte všetkých používateľov, s ktorými chcete politiku použiť, a potom vyberte položku **Upraviť** (ikona ceruzky).
8. V dialógovom okne kliknite na položku **funkcie poštovej schránky**. V časti **politika uchovávania údajov** použite politiku, ktorú ste práve vytvorili > **Uložiť**.
9. Pokyny na použitie politiky pre všetkých používateľov nájdete v téme [Použitie politiky uchovávania údajov v poštových schránkach](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
