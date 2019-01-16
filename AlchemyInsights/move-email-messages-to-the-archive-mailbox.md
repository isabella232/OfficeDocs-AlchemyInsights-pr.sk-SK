---
title: Presunúť e-mailových správ do archívnej poštovej schránky
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311754"
---
Problémy pri archivácii sa položky do archívnej poštovej schránky. Uistite sa, že ste vykonali nasledujúce kroky:
  
1. Potvrdiť, že bola povolená **archivácia poštovej schránky** . Ak nie, použite kroky v [tomto článku](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) na zapnutie archívnej poštovej schránky. 
    
2. V službe Exchange Admin Center, vyberte **Značky uchovávania údajov** podľa **Riadenia dodržiavania súladu**, vytvoriť **značku uchovávania údajov** s **premiestniť do archívu** akcie obsahujúce požadované **Obmedzenie veku uchovávania**.
    
3. Exchange Admin Center, vyberte **Politiky uchovávania údajov**, vytvoriť **Politiku uchovávania údajov** a pridať vaše **premiestniť do archívu** značky uchovávania údajov do tejto politiky. 
    
4. [Priradenie politiky uchovávania údajov](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštovej schránky špecifické používateľa. **Primárnej** a **archívnej** poštovej schránky sa použije rovnakú politiku. 
    
Poštová schránka používateľa teraz mali mať politiku archivácie premiestnite položky do archívnej poštovej schránky. Môže byť potrebné prinútiť podarilo priečinka asistent (MFA) spustiť a použiť nové nastavenia do poštovej schránky používateľa. Spustite nasledujúci príkaz zároveň [pripojený k EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spustiť Asistenta pre spravované priečinky v konkrétnej poštovej schránke: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Chcete sa dozvedieť viac o nastavení politiku archivácie, pozri [nastaviť Archív a odstránenie politiky poštových schránok](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

