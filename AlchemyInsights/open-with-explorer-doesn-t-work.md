---
title: Otvoriť v programe Prieskumník nefunguje
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713049"
---
# <a name="open-with-explorer-isnt-working"></a>Otvoriť v programe Prieskumník nefunguje

Ak **Otvoriť v programe Prieskumník** alebo **Zobraziť v Prieskumníkovi** nefunguje uistite sa, že služba WebClient je nastavená na **spúšťanie** podľa nasledujúcich krokov. Napríklad, to môže trvať dlho otvoriť SharePoint alebo OneDrive knižnice, keď služba nie je spustená. 
  
1. Do poľa Hľadať v systéme Windows zadajte príkaz Spustiť, vyberte položku spustiť počítačovú aplikáciu, zadajte príkaz Services. msc a potom vyberte položku **Enter (zadať**).
    
2. Posuňte sa nadol na službu WebClient a skontrolujte **stavový** stĺpec. Ak stav služby WebClient nie je **spustená**, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**, a potom kliknite na **tlačidlo OK**. Ak je to potrebné, povoľte službu výberom položky **manuálne** alebo **automaticky** v poli **Typ spustenia** . 
    
> [!NOTE]
> Ak chcete riešiť problémy s otvorením v Prieskumníkovi, pozrite si tému [Otvorenie v Prieskumníkovi](https://go.microsoft.com/fwlink/?linkid=871665). Preskúmajte synchronizáciu ako lepšiu alternatívu: [Synchronizujte súbory SharePoint s novým klientom synchronizácie služby OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

