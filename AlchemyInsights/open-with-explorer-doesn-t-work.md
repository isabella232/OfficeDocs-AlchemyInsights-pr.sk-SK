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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011351"
---
# <a name="open-with-explorer-isnt-working"></a>Program Otvoriť v programe Prieskumník nefunguje

Ak **príkaz Otvoriť v programe** **Prieskumník** alebo Zobraziť v Prieskumníkovi nefunguje, uistite sa, že služba WebClient je nastavená na položku Spustené pomocou nižšie uvedených krokov.  Otvorenie knižnice dokumentov alebo knižnice dokumentov môže trvať SharePoint OneDrive vtedy, keď služba nie je spustená. 
  
1. Do vyhľadávacieho Windows vyhľadávania zadajte výraz spustiť, vyberte počítačovú aplikáciu Spustiť, zadajte reťazec services.msc a potom vyberte položku **Zadať**.
    
2. Posuňte sa nadol do služby WebClient a skontrolujte **stĺpec** Stav. Ak stav služby WebClient nie je **Spustený,** dvakrát kliknite na službu, kliknite na tlačidlo **Štart** a potom na tlačidlo **OK.** Ak je to potrebné, povoľte službu výberom **možnosti** **Manuálne** alebo Automaticky v **poli Typ spustenia.** 
    
> [!NOTE]
> Ak chcete vyriešiť problémy pri otváraní v Prieskumníkovi, pozrite si [tému Otvoriť v programe Prieskumník.](https://go.microsoft.com/fwlink/?linkid=871665) Preskúmajte synchronizáciu ako lepšiu alternatívu: [SharePoint súborov pomocou nového synchronizačná aplikácia OneDrivu klienta](https://go.microsoft.com/fwlink/?linkid=871666). 
  

