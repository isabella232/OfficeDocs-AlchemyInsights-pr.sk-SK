---
title: Otvoriť v programe Prieskumník nefunguje
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
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694471"
---
# <a name="open-with-explorer-isnt-working"></a>Otvoriť v programe Prieskumník nefunguje

Ak je položka otvoriť v programe **Prieskumník** alebo **zobrazenie v Prieskumníkovi** funkčná, uistite sa, že služba WebClient je nastavená na možnosť **Spustiť** podľa nižšie uvedených krokov. Pri otváraní knižnice SharePointu alebo OneDrivu môže napríklad trvať dlho, kým nie je spustená služba. 
  
1. Do poľa Windows Search zadajte text spustiť, vyberte položku spustiť počítačovú aplikáciu, zadajte výraz Services. msc a potom vyberte položku **Enter**.
    
2. Posuňte sa nadol na službu WebClient a skontrolujte stĺpec **stav** . Ak stav služby WebClient nie je **spustený**, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom kliknite na tlačidlo **OK**. Ak je to potrebné, zapnite službu tak, že vyberiete možnosť **manuálne** alebo **Automatické** v poli **Typ spustenia** . 
    
> [!NOTE]
> Ak chcete riešiť problémy pri otváraní v Prieskumníkovi, pozrite si tému [Otvorenie v Prieskumníkovi](https://go.microsoft.com/fwlink/?linkid=871665). Preskúmajte synchronizáciu ako lepšiu alternatívu: [Synchronizujte súbory SharePointu s novým synchronizačným klientom pre OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

