---
title: Riešenie problémov s použitím funkcie otvoriť v programe Prieskumník
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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659073"
---
# <a name="fix-problems-with-open-with-explorer"></a>Riešenie problémov s otvorením v programe Prieskumník

Riešenie bežných problémov s otvorením knižnice dokumentov v SharePointe alebo vo OneDrive pomocou príkazu **Otvoriť v programe Prieskumník** : 
  
- Použite Internet Explorer 10 alebo Internet Explorer 11. **Otvoriť v programe Prieskumník** nie je kompatibilný s prehliadačom Microsoft Edge, Google Chrome, Firefox a ďalšími používateľmi. **Otvoriť v programe Prieskumník** je vo všetkých prehliadačoch zakázaný okrem programu Internet Explorer. 
    
- **Otvoriť v programe Prieskumník** nie je k dispozícii v modernom prostredí knižníc SharePointu. Namiesto toho použite **zobrazenie v Prieskumníkovi** . Vyberte zobrazenie **Možnosti zobrazenia** \> **v Prieskumníkovi**. Zobrazenie v Prieskumníkovi nie je kompatibilné s prehliadačom Microsoft Edge, Google Chrome, Firefoxom a ďalšími používateľmi. **Zobrazenie v Prieskumníkovi** je k dispozícii len v Internet Exploreri. 
    
- Skontrolujte, či je spustená služba WebClient. Do poľa Windows Search zadajte text spustiť, vyberte položku spustiť počítačovú aplikáciu, zadajte výraz Services. msc a potom stlačte kláves ENTER. Posuňte sa nadol na službu WebClient a skontrolujte, či sa v stĺpci **stav** zobrazuje text spustiť. Ak to tak nie je, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom na tlačidlo **OK**. (Ak chcete službu najskôr povoliť, vyberte možnosť **manuálne** alebo **Automatické** v poli **Typ spustenia** .) 
    
> [!NOTE]
> Otvorenie knižnice v Prieskumníkovi je užitočné v prípade, ak je potrebné skopírovať alebo premiestniť viacero súborov a priečinkov raz, ale ak chcete pravidelne pracovať v knižnici, odporúčame ju synchronizovať. Ak chcete riešiť problémy pri otváraní v Prieskumníkovi, pozrite si tému [Otvorenie v Prieskumníkovi](https://go.microsoft.com/fwlink/?linkid=871665). Informácie o nastavení synchronizácie nájdete v téme [Synchronizácia súborov SharePointu s novým synchronizačným klientom pre OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Ďalšie informácie nájdete v článku [používanie príkazu Otvoriť v programe Prieskumník na riešenie problémov v SharePointe Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) . 
  

