---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908724"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolenie šifrovania BitLocker pomocou Intune

 Intune Endpoint Protection politika môže byť použitá na konfigurovanie šifrovania BitLocker nastavenia pre zariadenia so systémom Windows. Ďalšie informácie nájdete v téme [Windows 10 (a novšie) nastavenia na ochranu zariadení pomocou služby Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Mali by ste si uvedomiť, že mnohé novšie zariadenia so systémom Windows 10 podporujú automatické šifrovanie BitLocker, ktoré sa spúšťa bez použitia politiky MDM. To môže ovplyvniť uplatňovanie politiky, ak nie sú predvolené nastavenia nakonfigurované. Ďalšie podrobnosti nájdete v nasledujúcich najčastejších otázkach.
 
Informácie o riešení problémov s šifrmi BitLocker nájdete [v téme Riešenie problémov s pravidlami šifrovania BitLocker v programe Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Najčastejšie otázky**

 Otázka: ktoré vydania systému Windows podporujú šifrovanie zariadenia pomocou politiky Endpoint Protection?<br>
 A: nastavenia v Intune Endpoint Protection politiky sú implementované pomocou [šifrovania BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nie všetky vydania alebo zostavy systému Windows podporujú šifrovanie BitLocker CSP. <br><br>
      V tomto okamihu sú podporované nasledujúce vydania systému Windows: Enterprise, Education, Mobile, Mobile Enterprise a Professional (build 1809 a novší).
 
Q: Ak zariadenie je už šifrované s BitLocker pomocou predvoleného nastavenia operačného systému pre metódu šifrovania a šifrovacia sila (XTS-AES-128), bude uplatňovať politiku s rôznymi nastaveniami automaticky spustí re-šifrovanie disku s novými nastaveniami?<br>
A: nie. Ak chcete použiť nové šifrovacie nastavenia, jednotka musí byť najprv dešifrovaná.<br><br>
**Poznámka:** Pre zariadenia, ktoré sa zaregistrujú s autopilot, automatické šifrovanie, ktoré by sa vyskytli počas OOBE sa nespúšťa, kým sa vyhodnotí politika Intune, čo umožňuje nastavenie založené na zásadách, ktoré sa použije namiesto predvolených hodnôt operačného systému.
 
Otázka: Ak je zariadenie šifrované v dôsledku uplatňovania politiky Intune, bude dešifrovať pri odstránení tejto politiky?<br>
A: Odstránenie politiky súvisiace s šifrovaním nemá za následok dešifrovanie jednotiek, ktoré boli nakonfigurované.
 
Otázka: prečo Intune súlad politiky ukazujú, že moje zariadenie nemá BitLocker povolené, aj keď to je?<br>
A: "BitLocker Enabled" nastavenie v Intune súladu politiky využíva Windows Device Health osvedčenie (DHA) klienta. Tento klient len meria stav zariadenia v čase spúšťania. Takže ak zariadenie nebolo reštartuje, pretože šifrovanie BitLocker bola dokončená, DHA klient služba nebude hlásiť BitLocker ako aktívny.
 
 