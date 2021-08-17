---
title: Oprava politiky pripojenia
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
- "9000760"
- "7391"
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314859"
---
# <a name="fix-connection-policy"></a>Oprava politiky pripojenia

E-mail bol označený ako bezpečný a doručený do priečinka doručenej pošty používateľa, pretože zdrojová IP adresa bola v predvolenej politike filtra pripojenia označená ako bezpečná. Ak si chcete politiku prekontrolovať, postupujte takto:

1. Na portáli Microsoft 365 Defender prejdite na položku Politiky spolupráce pre <https://security.microsoft.com/>  \>  \>  \> **e-&**  na & Pravidlá politiky hrozieb Ochrana pred nevyžiadanou poštou v časti Politiky.

   Ak chcete prejsť priamo na stránku **Politiky ochrany pred nevyžiadanou poštou,** <https://security.microsoft.com/antispam> použite .

2. Na stránke **Politiky ochrany pred nevyžiadanou** poštou kliknutím na názov politiky vyberte politiku s názvom Politika filtra pripojenia **(predvolené).**

3. V zobrazenej bubline podrobností kliknite v **časti Filtrovanie pripojenia na** položku Upraviť politiku **filtrovania** pripojenia.

4. Skontrolujte položky v časti **Vždy povoliť správy z** nasledujúcich IP adries alebo rozsahu adries a pozrite sa, či je **vybratá možnosť Zapnúť bezpečné.**

   **Poznámka:** Spoločnosť Microsoft má predplatné na zdroje dôveryhodných odosielateľov tretích strán. Ak je zoznam dôveryhodných odosielateľov povolený, títo dôveryhodní odosielatelia omylom nie sú označení ako nevyžiadaná pošta. Odporúčame vybrať túto možnosť, pretože sa zníži počet nesprávne pozitívnych e-mailov ( dobrej pošty, ktorá sa klasifikuje ako nevyžiadaná pošta), ktorú dostanete.

Ďalšie informácie nájdete v téme [Konfigurácia filtrovania pripojenia.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
