---
title: Chýbajúce podmienky v ukladacom priestore SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053528"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolenie šifrovania BitLocker pomocou Intune

Intune Endpoint Protection politiky môžu byť použité na konfigurovanie Boitlocker nastavenia šifrovania pre zariadenia so systémom Windows, ako je opísané v: windows10 (a novšie) nastavenia na ochranu zariadení pomocou Intune

Mali by ste si uvedomiť, že mnohé novšie zariadenia so systémom Windows 10 podporujú automatické šifrovanie BitLocker, ktoré sa spúšťa bez použitia politiky MDM. To môže ovplyvniť uplatňovanie politiky, ak nie sú nakonfigurované predvolené nastavenia. Ďalšie podrobnosti nájdete v téme Najčastejšie otázky.


FAQ  Q: ktoré vydania systému Windows podporuje šifrovanie zariadenia pomocou Endpoint Protection Policy?
 A: nastavenia v Intune Endpoint Protection politiky sú implementované pomocou šifrovania BitLocker CSP.Nie všetky vydania ani zostavy systému Windows podporujú šifrovanie BitLocker CSP. 
      V tomto okamihu vydania systému Windows: Enterprise; Vzdelávanie, mobilné, mobilné podnikanie a profesionálne (od Build 1809 ďalej) sú podporované.




Q: Ak zariadenie je už šifrované s BitLocker pomocou predvoleného nastavenia operačného systému pre metódu šifrovania a šifrovacia sila (XTS-AES-128) bude uplatňovať politiku s rôznymi nastaveniami automaticky spustí re-šifrovanie disku s novými nastaveniami?

A: nie. Ak chcete použiť nové nastavenie šifrovania, jednotka musí byť najprv dešifrovaná.

Poznámka: pre zariadenia, ktoré sa zaregistrujú s autopilot automatické šifrovanie, ktoré by sa vyskytli počas OOBE nie je spustená, kým sa vyhodnotí politika Intune, ktorá umožňuje politiky založené nastavenia použiť namiesto predvolené OS




Q Ak je zariadenie šifrované v dôsledku uplatňovania politiky Intune bude dešifrovať pri odstránení tejto politiky?

A: odstránenie šifrovania súvisiace politiky nemá za následok dešifrovanie jednotiek, ktoré boli nakonfigurované.




Otázka: prečo Intune súlad politiky ukazujú, že moje zariadenie nemá "BitLocker Enabled", ale to je?

A: "BitLocker Enabled" nastavenie v Intune súladu politiky využíva Windows Device Health osvedčenie (DHA) klienta. Tento klient len meria stav zariadenia v čase spúšťania. Takže ak zariadenie nebolo reštartuje, pretože šifrovanie BitLocker bola dokončená služba DHA klient nebude hlásiť BitLocker ako aktívny.