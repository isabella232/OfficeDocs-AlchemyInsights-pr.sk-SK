---
title: Politiky uchovávania údajov v Centre spravovania pre Exchange nefunguje
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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522822"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Politiky uchovávania údajov v Centre spravovania pre Exchange

Ak chcete, aby sme spúšťali automatizované kontroly nastavení uvedených nižšie, vyberte tlačidlo späť < -- v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s politikami uchovávania údajov.

 **Problém:** Novovytvorené alebo aktualizované politiky uchovávania údajov v Centre spravovania pre Exchange sa nevzťahujú na poštové schránky alebo položky sa nepremiestňujú do archívnej poštovej schránky alebo odstránené. 
  
 **Príčiny:**
  
- Môže to byť spôsobené **tým, že Asistent pre spravované** priečinky nespracuje poštovú schránku používateľa. Asistent pre spravované priečinky sa pokúša spracovať každú poštovú schránku v organizácii typu cloud raz za sedem dní. Ak zmeníte značku uchovávania údajov alebo použijete inú politiku uchovávania údajov pre poštovú schránku, môžete počkať, kým asistent pre spravované priečinky spracuje poštovú schránku, alebo môžete spustiť rutinu cmdlet Start-ManagedFolderAssistant a spustiť Asistenta pre spravované priečinky na spracovanie konkrétnej poštovej schránky. Spustenie tejto rutiny cmdlet je užitočné na testovanie alebo riešenie problémov s nastavením politiky uchovávania údajov alebo značky uchovávania údajov. Ďalšie informácie nájdete v časti [Spustenie Asistenta pre spravované priečinky](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Riešenie:** Spustite nasledujúci príkaz na spustenie Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Táto možnosť sa môže vyskytnúť aj v **prípade, že uchovávanie** údajov **bolo povolené v** poštovej schránke. Ak poštová schránka bola umiestnená na RetentionHold, politiky uchovávania údajov v poštovej schránke sa počas tohto obdobia nespracujú. Ďalšie informácie o nastavení retentionhold nájdete v téme: Zadržanie [uchovávania údajov poštovej schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Riešenie:**
    
  - Skontrolujte stav RetentionHold nastavenie konkrétnej poštovej schránky v [exo powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Spustite nasledujúci príkaz vypnúť RetentionHold **na** konkrétne poštovej schránky:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Teraz znova spustite Asistenta pre spravované priečinky:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Upozornenie:** Ak poštová schránka je menšia ako 10 MB, Asistent pre spravované priečinky automaticky spracovať poštovú schránku.
 
Ďalšie informácie o politikách uchovávania údajov v Centre spravovania pre Exchange nájdete v téme:
- [Značky uchovávania údajov a politiky uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Použitie politiky uchovávania údajov v poštových schránkach](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Pridanie alebo odstránenie značiek uchovávania údajov](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Ako identifikovať typ zadržania umiestneného v poštovej schránke](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
