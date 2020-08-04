---
title: Profily Wi-Fi intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555813"
---
# <a name="intune-wi-fi-profiles"></a>Profily Wi-Fi intune

Úspešná implementácia Wi-Fi pripojenia pre KLIENTOV MDM závisí od správne nasadený profil, ktorý odráža požiadavky podnikovej Wi-Fi infraštruktúry. Ak chcete skontrolovať príslušné nastavenia pre klientske platformy, ktoré vyšetrujete, nájdete v téme: 

[Pridanie nastavení Wi-Fi pre zariadenia so systémom Android v službe Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Pridanie nastavení Wi-Fi pre zariadenia určené pre Android Enterprise a plne spravované zariadenia v službe Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Pridanie nastavení Wi-Fi pre zariadenia so systémom iOS a iPadOS v službe Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Pridanie nastavení Wi-Fi pre Windows 10 a novšie zariadenia v službe Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Import nastavení Wi-Fi pre zariadenia so systémom Windows v programe Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Bežné problémy**

**Nasadzujem profil Wi-Fi, ktorý je závislý od nasadeného certifikátu zadaného v profile Wi-Fi. Konfiguračné profily však zobrazujú stav chyby.**

Skontrolujte, či vaše zariadenie prijalo certifikát.

1. V časti Intune prejdite **na položku Všetky** zariadenia a vyberte > **zariadenia**.

2. Skontrolujte, či všetky očakávané profily sú uvedené a v úspešnom stave.

3. Ak máte v reťazci certifikátov dočasné certifikáty, v prípade profilu Android sa uistite, že sú nasadené do zariadení s Androidom.

    Ak chcete skontrolovať stav certifikátu, prejdite na **Profily konfigurácie**  >  **zariadenia**  >  **Android stredne CA Vlastnosti**  >  **dôveryhodný**  >  **certifikát**.

Ak sa chyby naďalej vyskytujú, prečítajte si postupy a časti na riešenie problémov. Ďalšie informácie nájdete v téme Prehľad [riešenia problémov s profilmi certifikátov SCEP s Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Nasadel som profil Wi-Fi do zariadenia. Intune ukazuje, že to bolo úspešné, ale zariadenie nie je pripojenie k Wi-Fi.**

Úspešný stav znamená, že intune úspešne nasadil profil nakonfigurovaný. Tieto konfigurácie sa však nemusia zhodovať s požiadavkami na sieť a alebo overenie. Ďalšie podrobnosti o pokuse o pripojenie, skontrolujte denníky v infraštruktúre a overovacia služba (na radiči bodu Prístupu Wi-Fi a NPS/Radius server). Na zhromažďovanie a kontrolu denníkov môže byť potrebné spolupracovať s tímom sieťovej infraštruktúry alebo s dodávateľom Wi-Fi tretej strany.