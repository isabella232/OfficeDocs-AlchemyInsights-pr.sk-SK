---
title: Vyhľadanie IP adresy v denníku auditu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902275"
---
# <a name="find-the-ip-address-in-audit-log"></a>Vyhľadanie IP adresy v denníku auditu

IP adresa, ktorá zodpovedá aktivite vykonanej používateľom alebo správcom, sa zobrazí v denníkoch auditu. Zapíšu sa aj informácie o klientovi. TU je postup na identifikáciu IP adresy:

1. Vykonajte jednu z nasledujúcich akcií:
   - V časti Centrum dodržiavania súladu pre Microsoft 365 prejdite <https://compliance.microsoft.com> na položku **Kontrola** \> **riešení.** Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portáli Microsoft 365 Defender prejdite <https://security.microsoft.com> na položku **Audit**. Alebo ak chcete prejsť priamo na **stránku Auditu,** použite <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Ak sa zobrazí upozornenie, že potrebujete zapnúť auditovanie, pokračujte a zapnite ho teraz. Ak táto funkcia nie je povolená, výsledky hľadania nebudú môcť získať údaje z predchádzajúcich dátumov.

2. Na stránke **Audit** overte, či **je vybratá** karta Hľadať, a potom nakonfigurujte tieto nastavenia:
   - **Rozsah dátumu a času:** Vyberte rozsah dátumu a času v **poliach Začiatok** **a** Koniec.
   - **Aktivity:** Ak máte záujem o konkrétnu aktivitu, vyberte ju v zozname; V opačnom prípade sa vráti **predvolená hodnota Zobraziť výsledky pre** všetky aktivity, všetky aktivity. Všimnite si, že niektoré činnosti možno nebudú k dispozícii na výber. Tieto položky auditu sa však vrátia, ak **vyberiete položku Zobraziť výsledky pre** všetky aktivity.
   - **Používatelia:** Prijmite prázdnu predvolenú hodnotu, aby sa vrátili výsledky pre všetkých používateľov, alebo zadajte jedného alebo viacerých používateľov.

3. Po dokončení kliknite na tlačidlo **Hľadať**. Aktivity sa zobrazia na novej **stránke Auditovanie.**

4. Vo výsledkoch kliknite na položku **Filtrovať výsledky** a do poľa filtra aktivity zadajte text **Set-Mailbox.**

5. Výberom záznamu auditu vo výsledkoch otvorte **leták** Podrobnosti.

Ďalšie informácie nájdete v téme [Vyhľadávanie v denníku auditu a preskúmanie bežných problémov technickej podpory.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
