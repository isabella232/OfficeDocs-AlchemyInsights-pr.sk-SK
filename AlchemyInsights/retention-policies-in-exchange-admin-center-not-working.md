---
title: Politiky uchovávania údajov v Exchange Admin Center nefunguje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489067"
---
 **Problém:** Novo vytvorené alebo aktualizované Retenčná politika v centre výmenu Admin nie sú uplatnenie k poštovým schránkam alebo položky nie sú presunuté do archívnej poštovej schránky alebo odstránené. 
  
 **Príčiny:**
  
- To môže byť, pretože **Asistent spravovaných priečinkov** nebola spracovaná poštovej schránky používateľa. Asistent pre spravované priečinky snaží spracovať každú poštovú schránku organizácii cloud raz za každých sedem dní. Ak zmeníte značku uchovávania údajov alebo použijete pre poštovú schránku inú politiku uchovávania údajov, môžete počkať, kým riadené priečinok Assist spracuje údaje poštovej schránky, alebo môžete spustiť Štart-ManagedFolderAssistant cmdlet spustiť Asistenta pre spravované priečinky spracovať konkrétne Poštová schránka. Spustenie tejto rutiny cmdlet je užitočné pri testovaní politiky uchovávania údajov a nastavení značky uchovávania údajov pri riešení problémov. Pre viac informácií, navštívte [Spustenie Asistenta pre spravované priečinky](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Riešenie:** Spustite nasledovný príkaz na spustenie Asistenta pre spravované priečinky v konkrétnej poštovej schránke: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To môže nastať aj ak **RetentionHold** bolo **zapnuté** poštovej schránky. Ak poštovú schránku bol kladený na RetentionHold, politiku uchovávania údajov poštovej schránky nebudú spracované počas tejto doby. Pre ďalšie informácie pozri Nastavenie RetentionHold: [Zadržania uchovávania údajov poštovej schránky](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    Riešenie
    
  - Skontrolujte stav RetentionHold nastavenia špecifické schránky v [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Spustite nasledujúci príkaz **vypnúť** RetentionHold na špecifické schránky: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Teraz znova spustiť spravované priečinok asistent:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Poznámka:** Ak poštová schránka je menšie ako 10 MB, Asistent pre spravované priečinky automaticky nespracováva poštovú schránku. 
  

