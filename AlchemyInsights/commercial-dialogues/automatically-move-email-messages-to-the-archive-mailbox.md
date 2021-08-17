---
title: Automatické premiestnenie e-mailových správ do archívnej poštovej schránky
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
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059241"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatické premiestnenie e-mailových správ do archívnej poštovej schránky

Postup nastavenia politiky automatického premiestnenia starých e-mailov používateľa do archívnej poštovej schránky:

1. Prejdite na [**kartu & Riadenie údajov**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Archív a overte, či používateľovi bola povolená  >    >   archívna poštová schránka. Ak nie, kliknite na položku Povoliť **a potom v** poli **s** upozornením na možnosť Áno.
2. Prejdite do [**Exchange spravovania > spravovania súladu > značky uchovávania údajov**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Vyberte ikonu + a potom položku automaticky **použiť na celú poštovú schránku**.
4. K značke uchovávania údajov priraďte názov a vyberte položku **Premiestniť do archívu.** Pre obdobie uchovávania zadajte čas, ktorý chcete, napríklad 90 dní. Kliknite na tlačidlo **Uložiť**.
5. Teraz vytvorte politiku uchovávania údajov: vyberte **položku Politiky uchovávania** údajov , výberom ikony pridajte novú politiku.
6. Priraďte názov k politike uchovávania údajov, kliknite na túto položku a posúvaním ju vyhľadajte a pridajte značku uchovávania údajov, ktorú ste práve vytvorili. Kliknite na tlačidlo **Uložiť**.
7. Nakoniec použite politiku uchovávania údajov pre poštovú schránku používateľa: v Centre spravovania pre Exchange prejdite na položku Poštové **schránky**  >  **príjemcov**. Vyberte všetkých používateľov, na ktorých chcete použiť politiku, a potom vyberte položku **Upraviť** (ikona ceruzky).
8. V dialógovom okne kliknite na položku Funkcie **poštovej schránky.** V **časti Politika uchovávania** údajov použite politiku, ktorú ste práve vytvorili > **Uložiť**.
9. Pokyny na použitie politiky pre všetkých používateľov nájdete v téme [Použitie politiky uchovávania údajov na poštové schránky.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
