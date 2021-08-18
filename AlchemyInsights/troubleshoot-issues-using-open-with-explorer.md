---
title: Riešenie problémov pomocou príkazu Otvoriť v programe Prieskumník
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323581"
---
# <a name="fix-problems-with-open-with-explorer"></a>Riešenie problémov s programom Otvoriť v programe Prieskumník

Riešenie bežných problémov s otvorením knižnice dokumentov v SharePoint alebo OneDrive pomocou **príkazu Otvoriť v programe** Prieskumník: 
  
- Použite Internet Explorer 10 alebo Internet Explorer 11. **Možnosť Otvoriť v programe** Prieskumník nie je kompatibilná s Microsoft Edge, Google Chrome, Firefox a ďalšími. **Možnosť Otvoriť v programe Prieskumník** je vypnutá vo všetkých prehliadačoch okrem Internet Explorera. 
    
- **Verzia Otvoriť v programe** Prieskumník nie je v modernom nastavení pre SharePoint knižnice k dispozícii. Namiesto **toho použite zobrazenie v Prieskumníkovi.** Vyberte **položku Zobraziť možnosti** Zobraziť v \> **Prieskumníkovi**. Zobrazenie v Prieskumníkovi nie je kompatibilné s Microsoft Edge, Google Chrome, Firefox a ďalšími. **Zobrazenie v Prieskumníkovi je k** dispozícii len v Internet Exploreri. 
    
- Uistite sa, že služba WebClient je spustená. Do vyhľadávacieho Windows vyhľadávania zadajte výraz spustiť, vyberte počítačovú aplikáciu Spustiť, zadajte reťazec services.msc a potom stlačte kláves Enter. Posuňte sa nadol na službu WebClient a skontrolujte, či sa v **stĺpci Stav** zobrazuje "Running" (Spustené). Ak sa tak nespustí, dvakrát kliknite na službu, kliknite na **tlačidlo Spustiť** a potom kliknite na tlačidlo **OK.** (Možno bude potrebné najprv službu zapnúť výberom **možnosti** Manuálne alebo **Automaticky** v poli **Typ spustenia.)** 
    
**Poznámka:** Otvorenie knižnice v Prieskumníkovi je užitočné, ak potrebujete skopírovať alebo premiestniť viacero súborov a priečinkov raz, ale ak chcete v knižnici pravidelne pracovať, odporúčame ju synchronizovať. Ak chcete vyriešiť problémy pri otváraní v Prieskumníkovi, pozrite si [tému Otvoriť v programe Prieskumník.](https://go.microsoft.com/fwlink/?linkid=871665) Informácie o nastavení synchronizácie nájdete v téme [Synchronizácia SharePoint pomocou nového klienta synchronizačná aplikácia OneDrivu synchronizácie.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Ďalšie informácie nájdete v článku Použitie príkazu Otvoriť v programe Prieskumník na riešenie problémov [v SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
  

