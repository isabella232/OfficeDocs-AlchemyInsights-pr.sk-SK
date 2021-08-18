---
title: Otvorenie v Prieskumníkovi nefunguje
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321876"
---
# <a name="open-with-explorer-isnt-working"></a>Program Otvoriť v programe Prieskumník nefunguje

Ak **príkaz Otvoriť v programe** **Prieskumník** alebo Zobraziť v Prieskumníkovi nefunguje, uistite sa, že služba WebClient je nastavená na položku Spustené pomocou nižšie uvedených krokov.  Otvorenie knižnice dokumentov alebo knižnice dokumentov môže trvať SharePoint ako OneDrive vtedy, keď služba nie je spustená. 
  
1. Do vyhľadávacieho Windows vyhľadávania zadajte výraz spustiť, vyberte počítačovú aplikáciu Spustiť, zadajte reťazec services.msc a potom vyberte položku **Zadať**.
    
2. Posuňte sa nadol do služby WebClient a skontrolujte **stĺpec** Stav. Ak stav služby WebClient nie je **Spustený,** dvakrát kliknite na službu, kliknite na tlačidlo **Štart** a potom na tlačidlo **OK.** Ak je to potrebné, povoľte službu výberom **možnosti** **Manuálne** alebo Automaticky v **poli Typ spustenia.** 
    
**Poznámka:** Ak chcete vyriešiť problémy pri otváraní v Prieskumníkovi, pozrite si [tému Otvorenie v Programe Prieskumník.](https://go.microsoft.com/fwlink/?linkid=871665) Preskúmajte synchronizáciu ako lepšiu alternatívu: [SharePoint súborov pomocou nového synchronizačná aplikácia OneDrivu klienta](https://go.microsoft.com/fwlink/?linkid=871666). 
  

