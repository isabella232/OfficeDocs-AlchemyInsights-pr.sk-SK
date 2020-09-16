---
title: Problémy s licenciou Yammer
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657291"
---
# <a name="yammer-licensing-issues"></a>Problémy s licenciou Yammer

Všetci používatelia musia mať licenciu na používanie podnikovej služby Yammer, ale predvolene Yammer nevyžaduje, aby mali používatelia licenciu na prístup k službe. Keď správca zmení nastavenie tak, aby blokoval používateľov služieb Microsoft 365 bez licencií na Yammer, používatelia, ktorí nemajú priradenú licenciu na Yammer Enterprise, nemôžu získať prístup k službe Yammer. Ďalšie informácie nájdete v téme [Správa používateľských licencií yammera v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Keď sa licencie odstránia od používateľov, dlaždica Yammer sa už nezobrazuje a ďalšie služby môžu pomocou odstraňovania licencií použiť na skrytie funkcií. V iných prípadoch sa funkcie môžu naďalej zobrazovať, ale vyžadujú, aby sa na ňu vyžadovalo nasadenie licencií.  

**Licencia sa používateľovi neaktualizuje**  

Niekedy je používateľovi priradená licencia, ale stále nie je možné získať prístup k Yammeru. Oneskorenie je pravdepodobnejšie, keď prebieha pridelenie hromadnej licencie. Používatelia yammera sa nemusia aktualizovať v rovnakom poradí, v akom sa licencie zmenia v službe Azure AD, pretože systém funguje asynchrónne. Počkajte až 24 hodín, kým sa neotvorí prípad podpory, aby sa nahlásili problémy so synchronizáciou licencií.  

**Priradenie hromadnej licencie**  

Licencie je možné priradiť prostredníctvom centra spravovania alebo skriptovania v prostredí PowerShell. Ďalšie informácie nájdete v téme [Priradenie licencií používateľom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a [Priradenie licencií k používateľským kontám v prostredí Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Technická podpora spoločnosti Microsoft neposkytuje pomoc pri vytváraní skriptov, ale dokumentácia o priradení licencií na Yammer je k dispozícii. Ďalšie informácie nájdete v téme [Správa licencií na Yammer pomocou prostredia Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).