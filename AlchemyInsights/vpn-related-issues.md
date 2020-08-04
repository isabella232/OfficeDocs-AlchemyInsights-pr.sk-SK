---
title: Problémy súvisiace s VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555746"
---
# <a name="vpn-related-issues"></a>Problémy súvisiace s VPN

Úspešná implementácia pripojenia VPN pre klientov MDM závisí od nasadený profil, ktorý správne odráža požiadavky infraštruktúry VPN. Príslušné nastavenia pre klientske platformy, ktoré vyšetrujete, nájdete v téme: 

[Nastavenia holografického zariadenia vo Windowse 10 a Windowse na pridanie pripojení VPN pomocou aplikácie Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Pridanie nastavení VPN v zariadeniach so systémom iOS a iPadOS v službe Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Nastavenia zariadenia android na konfiguráciu VPN v Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Pridanie nastavení VPN v zariadeniach so systémom macOS v službe Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Ak váš vpn profil používa overovanie na základe certifikátu, uistite sa, že koreňový certifikát a klient overovanie certifikát profily prepojené s vpn profil sú úspešne nasadené.

**Bežné problémy**

**Nasadil som vpn profil do zariadenia. Intune ukazuje, že to bolo úspešné, ale zariadenie nie je pripojenie k VPN.**

Úspešný stav znamená, že intune úspešne nasadil profil nakonfigurovaný. Tieto konfigurácie sa však nemusia zhodovať s požiadavkami na sieť a alebo overenie. Skontrolujte denníky v infraštruktúre a overovacia služba (na serveri VPN a NPS/Radius server) pre viac informácií o pokuse o pripojenie. Na zhromažďovanie a kontrolu denníkov môže byť potrebné spolupracovať s tímom sieťovej infraštruktúry alebo s dodávateľom siete VPN tretej strany.

**Pri konfigurácii vlastnej siete VPN pre systém iOS nie je k dispozícii funkcia VPN pre vlastnú aplikáciu.**

Vpn pre zariadenia so systémom iOS v aplikácii Intune je momentálne k dispozícii pre konkrétny zoznam poskytovateľov a partnerov, ktorí musia pred konfiguráciou vpn pre jednotlivé aplikácie spĺňať aj požiadavky na certifikát. Ďalšie informácie nájdete v téme [Nastavenie virtuálnej súkromnej siete (VPN) pre zariadenia so systémom iOS/iPadOS v programe Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Ďalšie informácie o všetkých typoch pripojení VPN v programe Intune nájdete v téme [Vytvorenie profilov VPN na pripojenie k serverom VPN v programe Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**iOS On-Demand VPN sa neštuduje pri prístupe k nakonfigurovanej doméne**

Ak chcete otestovať automatické nastavenie siete VPN, nastavte nasledujúce hodnoty:

Chcem urobiť nasledovné: Vyhodnoťte **každý pokus o pripojenie** 

Vyberte, či sa chcete pripojiť: **V prípade potreby sa pripojte**

Keď používatelia pristupujú k týmto doménam: **názov** *cieľovej domény*

Ak vyššie uvedená konfigurácia nie je úspešná, pridajte nasledujúci prvok:

Ak je táto adresa URL nedosiahnuteľná, vynútiť pripojenie vpn: **BADURL**