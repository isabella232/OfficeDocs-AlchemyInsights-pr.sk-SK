---
title: Politiky uchovávania údajov v centre spravovania pre Exchange nefunguje
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740525"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Politiky uchovávania údajov v centre spravovania pre Exchange

Ak chcete, aby sme spustili automatizované kontroly nižšie uvedených nastavení, vyberte tlačidlo späť < – v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s politikami uchovávania údajov.

 **Problém:** Novo vytvorené alebo aktualizované politiky uchovávania údajov v centre spravovania pre Exchange sa nevzťahujú na poštové schránky ani položky, ktoré nie sú presunuté do archívnej poštovej schránky alebo odstránené. 
  
 **Hlavné príčiny:**
  
- Môže to byť spôsobené tým, že **asistent pre spravované priečinky** nespracoval poštovú schránku používateľa. Asistent pre spravované priečinky sa po každých siedmich dňoch pokúsi spracovať každú poštovú schránku v organizácii využívajúcej cloud. Ak zmeníte značku uchovávania údajov alebo použijete inú politiku uchovávania údajov pre poštovú schránku, môžete počkať, kým spravovaný priečinok spracuje poštovú schránku, alebo môžete spustiť rutinu typu cmdlet Start-ManagedFolderAssistant a spustiť Asistenta pre spravované priečinky na spracovanie konkrétnej poštovej schránky. Spustenie tejto rutiny typu cmdlet je užitočné pri testovaní alebo riešení problémov s nastaveniami politiky uchovávania údajov alebo značky uchovávania údajov. Ďalšie informácie nájdete v téme [Spustenie Asistenta pre spravované priečinky](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Riešenie:** Spustite nasledujúci príkaz na spustenie Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Môže sa to vyskytnúť aj v prípade, ak je **RetentionHold** **zapnutá** v poštovej schránke. Ak je poštová schránka umiestnená na RetentionHold, politika uchovávania údajov v poštovej schránke sa počas tohto času nespracuje. Ďalšie informácie o inštalácii v nastaveniach RetentionHold nájdete v téme: [uchovanie poštovej schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Riešenie**
    
  - Skontrolujte stav nastavenia RetentionHold v konkrétnej poštovej schránke v [prostredí EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Spustite tento príkaz na **Vypnutie** RetentionHold v konkrétnej poštovej schránke:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Teraz znova spustite Asistenta pre spravované priečinky:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Poznámka:** Ak je poštová schránka menšia než 10 MB, Asistent pre spravované priečinky automaticky nespracuje poštovú schránku.
 
Ďalšie informácie o politikách uchovávania údajov v centre spravovania pre Exchange nájdete v témach:
- [Značky uchovávania údajov a politiky uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Použitie politiky uchovávania údajov v poštových schránkach](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Pridanie alebo odstránenie značiek uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Ako identifikovať typ zadržania umiestneného v poštovej schránke](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
