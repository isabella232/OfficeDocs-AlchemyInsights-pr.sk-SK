---
title: Problémy s licenciami yammera
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148320"
---
# <a name="yammer-licensing-issues"></a>Problémy s licenciami yammera

Všetci používatelia musia mať licenciu na používanie služby Yammer Enterprise, ale v predvolenom nastavení sieť Yammer nevyžaduje, aby používatelia mali licenciu na prístup k službe. Keď správca zmení nastavenie blokovať Microsoft 365 používateľov bez licencií yammera, používatelia nie je priradená yammer Enterprise licencie nemôže získať prístup k službe Yammer. Ďalšie informácie nájdete v téme [Správa používateľských licencií Yammera v službách Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Keď licencie sú odstránené od používateľov, yammer dlaždice sa už nezobrazuje a iné služby môžete použiť odstránenie licencie skryť funkcie. V ostatných prípadoch sa funkcie môžu stále zobrazovať, ale vyžadujú, aby licencia priradenie fungovalo.  

**Licencia sa neaktualizuje pre používateľa**  

Niekedy používateľ je priradená licencia, ale stále nie je schopný získať prístup k sieti Yammer. Oneskorenia sú pravdepodobnejšie, že dôjde, keď prebieha hromadné priradenie licencie. Používatelia yammera nemusia byť aktualizované v rovnakom poradí ako licencie sa zmenia v Azure AD, pretože systém beží asynchrónne. Počkajte až 24 hodín pred otvorením prípadu technickej podpory na hlásenie problémov so synchronizáciou licencie.  

**Hromadné pridelenie licencie**  

Licencie je možné priradiť prostredníctvom centra spravovania alebo skriptovania prostredia PowerShell. Ďalšie informácie nájdete v [témach Priradenie licencií používateľom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a [Priradenie licencií k používateľským kontám pomocou prostredia PowerShell služieb Office 365](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Technická podpora spoločnosti Microsoft neposkytuje pomoc pri vytváraní skriptov, ale k dispozícii je dokumentácia o priradení licencie yammera. Ďalšie informácie nájdete v téme [Správa licencií yammera pomocou prostredia Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).