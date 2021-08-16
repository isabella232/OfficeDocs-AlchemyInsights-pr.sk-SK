---
title: Yammer problémy s licenciou
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989750"
---
# <a name="yammer-licensing-issues"></a>Yammer problémy s licenciou

Všetci používatelia musia mať licenciu na používanie služby Yammer Enterprise, ale predvolene Yammer nevyžaduje, aby používatelia mali licenciu na prístup k službe. Keď správca zmení nastavenie blokovania Microsoft 365 používateľov bez Yammer, používatelia, ktorí nemajú priradenú licenciu na Yammer Enterprise, nebudú mať prístup Yammer služby. Ďalšie informácie nájdete v téme [Spravovanie Yammer používateľských licencií v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Po odobraní licencií používateľom sa už Yammer nezobrazuje a iné služby môžu na skrytie funkcií použiť odstránenie licencií. V iných prípadoch sa funkcie môžu naďalej zobrazovať, ale na prevádzku sa vyžaduje priradenie licencie.  

**Používateľovi sa neaktualizuje licencia**  

Niekedy je používateľovi priradená licencia, ale stále nemôže získať prístup k Yammer. Oneskorenia sa vyskytnú skôr, keď prebieha hromadné priradenie licencií. Yammer sa používatelia nemusia aktualizovať v rovnakom poradí ako licencie v Azure AD, pretože systém sa spúšťa asynchrónne. Ak chcete nahlásiť problémy so synchronizáciou licencií, počkajte do 24 hodín pred otvorením prípadu podpory.  

**Hromadné priradenie licencie**  

Licencie je možné priradiť prostredníctvom Centra spravovania alebo skriptovania v prostredí PowerShell. Ďalšie informácie nájdete v téme [Priradenie licencií používateľom a](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Priradenie licencií [k používateľským kontám pomocou Office 365 PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Podpora spoločnosti Microsoft neposkytuje pomoc s vytváraním skriptov, k dispozícii je však Yammer priradenie licencií. Ďalšie informácie nájdete v [téme Yammer licencií pomocou Windows PowerShell.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)