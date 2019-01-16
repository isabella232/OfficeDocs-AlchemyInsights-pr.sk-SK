---
title: Riešiť synchronizáciu hesla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311423"
---
# <a name="troubleshoot-password-synchronization"></a>Riešiť synchronizáciu hesla

Riešenie problémov, kde žiadne heslá sú synchronizované Azure AD pripojiť verziu 1.1.614.0 alebo novšiu verziu:
  
1. Otvorte novú reláciu prostredia Windows PowerShell na Azure AD pripojiť server pomocou možnosti **Spustiť ako správca** . 
    
2. Spustiť **Set-ExecutionPolicy RemoteSigned** alebo **Set-ExecutionPolicy neobmedzený**. 
    
3. Spustiť sprievodcu Azure AD pripojiť.
    
4. Prejdite na ** ďalšie úlohy ** stránky, vyberte ** riešenie **, a kliknite na tlačidlo **ďalej**. 
    
5. Na stránke Riešenie problémov kliknite na ponuku **spustenie na spustenie riešenia problémov** v prostredí PowerShell. 
    
6. V hlavnom menu, vyberte **Riešenie problémov synchronizácie heslo**. 
    
7. V podmenu vyberte **synchronizáciu hesla nefunguje vôbec**. 
    
 **Porozumieť výsledky riešenia úlohy**
  
Riešenie problémov úloha vykoná tieto kontroly:
  
- Overuje, že heslo synchronizácia zapnutá pre nájomcu Azure AD.
    
- Overuje, že Azure AD pripojiť server nie je v oddychových režime.
    
- Pre každý existujúci lokálneho Active Directory konektor (čo zodpovedá existujúcu aktívnu Adresárová štruktúra):
    
- 
  - Overuje, či je zapnutá funkcia synchronizácie heslo.
    
  - Vyhľadáva heslo synchronizácie tep udalostí v denníku udalostí aplikácie Windows.
    
  - Pre každú doménu služby Active Directory do lokálnej služby Active Directory konektor:
    
  - Overuje, že doména je dosiahnuteľný z server Azure AD pripojiť.
    
  - Overuje, že Active Directory Domain Services (AD DS) účty používané konektor služby Active Directory lokálne má správne meno používateľa, heslo a povolenia potrebné pre synchronizáciu hesla.
    
Viac pomoc riešenie problémov synchronizácie heslo nájdete v časti [Riešenie problémov heslo synchronizácia s Azure AD pripojenie synchronizácie](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

