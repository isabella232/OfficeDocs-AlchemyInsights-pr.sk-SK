---
title: Riešenie problémov s synchronizáciou hesla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732525"
---
# <a name="troubleshoot-password-synchronization"></a>Riešenie problémov s synchronizáciou hesla

Riešenie problémov, kde žiadne heslá sú synchronizované s Azure AD Connect verzie 1.1.614.0 alebo novšej:
  
1. Otvorte novú reláciu prostredia Windows PowerShell na serveri Azure AD Connect s možnosťou **Spustiť ako správca** .

2. Spustiť **súbor executionpolicy RemoteSigned** alebo **set-executionpolicy neobmedzený**.

3. Spustite Sprievodcu Azure AD Connect.

4. Prejdite na stránku **ďalšie úlohy** , vyberte **Riešenie problémov**a kliknite na tlačidlo **ďalej**.

5. Na stránke Riešenie problémov, kliknite na tlačidlo **Spustiť spustite ponuku riešenie problémov** v prostredí PowerShell.

6. V hlavnej ponuke vyberte položku **Riešenie problémov s synchronizáciou hesiel**.

7. V sub menu, vyberte **heslo synchronizácia nefunguje vôbec**.

**Pochopenie výsledkov úlohy pri riešení problémov**
  
Riešenie problémov úloha vykonáva nasledujúce kontroly:
  
- Overuje, či je zapnutá funkcia synchronizácie hesiel pre nájomcu Azure AD.

- Overuje, či server Azure AD Connect nie je v režime oddychové.

- Pre každý existujúci lokálny konektor služby Active Directory (ktorý zodpovedá existujúcej doménovej štruktúre služby Active Directory):

- 
  - Overuje, či je zapnutá funkcia synchronizácie hesiel.

  - Vyhľadáva heslo synchronizácia heartbeat udalosti v denníku udalostí aplikácie systému Windows.

  - Pre každú doménu služby Active Directory v lokálnom konektor služby Active Directory:

  - Overuje, či je doména dostupná zo servera Azure AD Connect.

  - Overuje, či kontá služby Active Directory Domain (AD DS), ktoré používa lokálny konektor služby Active Directory, má správne používateľské meno, heslo a povolenia potrebné na synchronizáciu hesla.

Ďalšie pomoc pri riešení problémov so synchronizáciou hesiel nájdete v téme [Riešenie problémov s synchronizáciou hesiel pomocou synchronizácie Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  