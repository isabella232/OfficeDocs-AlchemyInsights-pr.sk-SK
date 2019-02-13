---
title: Open s Explorer nefunguje
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906819"
---
# <a name="open-with-explorer-isnt-working"></a>Open s Explorer nefunguje

Ak **Otvoriť v programe Prieskumník** alebo **v Prieskumníkovi** nepomôže uistite sa, že služba WebClient nastavená na **Spustenie** pomocou nasledujúcich krokov. Napríklad to môže trvať dlhú dobu na otvorenie knižnice SharePoint alebo OneDrive, keď služba nie je spustená. 
  
1. Windows vyhľadávacieho poľa zadajte text spustiť, vyberte počítačovú aplikáciu spustiť, zadajte príkaz services.msc a potom stlačte **kláves Enter**.
    
2. Prejdite na službu WebClient a skontrolujte **stav** stĺpec. Ak stav služby WebClient nie je **spustený**, dvakrát kliknite na službu, kliknite na tlačidlo **Štart**a potom kliknite na tlačidlo **OK**. Zapnutie služby, v prípade potreby výberom **vybertemanuálne** alebo **Automatické** v poli **Typ spustenia** . 
    
> [!NOTE]
> Riešenie problémov otvoriť v programe Prieskumník, pozrite si [Otvoriť v programe Prieskumník](https://go.microsoft.com/fwlink/?linkid=871665). Preskúmajte synchronizácie ako lepšiu alternatívu: [synchronizovať SharePoint súbory pomocou nového klienta synchronizácie služby OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

