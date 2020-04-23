---
title: Politiky uchovávania údajov v Exchange Admin Center nepracuje
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742448"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Politiky uchovávania údajov v stredisku Exchange Admin Center

 **Problém:** Novovytvorené alebo aktualizované politiky uchovávania údajov Exchange Admin Center sa nevzťahujú na poštové schránky alebo položky sa nepremiestnia do archívnej poštovej schránky alebo odstránené. 
  
 **Príčiny:**
  
- Môže to byť spôsobené tým, že **asistent pre spravované priečinky** nespracoval poštovú schránku používateľa. Asistent pre spravované priečinky sa pokúša spracovať každú poštovú schránku v organizácii typu cloud raz za sedem dní. Ak zmeníte značku uchovávania údajov alebo použijete inú politiku uchovávania údajov pre poštovú schránku, môžete počkať, kým asistent spravovaných priečinkov spracuje poštovú schránku, alebo môžete spustiť rutinu cmdlet Start-ManagedFolderAssistant na spustenie Asistenta pre spravované priečinky na spracovanie konkrétnej poštovej schránky. Spustenie tejto rutiny cmdlet je užitočné pre testovanie alebo riešenie problémov politiky uchovávania údajov alebo nastavenia značky uchovávania údajov. Ďalšie informácie nájdete v téme [Spustenie Asistenta pre spravované priečinky](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Riešenie:** Spustite nasledovný príkaz na spustenie Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To môže nastať aj ak **RetentionHold** bola **povolená** v poštovej schránke. Ak poštová schránka bola umiestnená na RetentionHold, politika uchovávania údajov v poštovej schránke nebude spracovaná počas tohto času. Ďalšie informácie o nastavení RetentionHold nájdete: [zadržanie poštovej schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Riešenie:**
    
  - Skontrolujte stav RetentionHold nastavenie na konkrétnu poštovú schránku v [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Spustite nasledovný príkaz na **Vypnutie** RetentionHold na konkrétnu poštovú schránku:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Teraz znova spustite Asistenta pre spravované priečinky:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Poznámka:** Ak je poštová schránka menšia ako 10 MB, Asistent pre spravované priečinky nebude automaticky spracovávať poštovú schránku.
 
Ďalšie informácie o politikách uchovávania údajov v centre spravovania servera Exchange nájdete v téme:
- [Značky uchovávania údajov a politiky uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Použitie politiky uchovávania údajov pre poštové schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Pridanie alebo odstránenie značiek uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Ako identifikovať typ hold umiestnené v poštovej schránke](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
