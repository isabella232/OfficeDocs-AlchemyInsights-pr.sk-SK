---
title: Synchronizácia profilu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320724"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kedy sa moje zmeny profilu synchronizujú s aplikáciou SharePoint používateľských profilov?

SharePoint Online používa úlohu časovača importu služby Active Directory (AD Import) na importovanie používateľov a skupín do aplikácie používateľského profilu. 
  
1. Import služby AD synchronizuje zmeny z SharePoint online ukladacieho priestoru do aplikácie používateľských profilov. Tieto zmeny sa spracúvajú v dávkach.
    
2. Úloha časovača sa spustí dovtedy, kým sa zmeny nesynchronizujú.
    
**Poznámka:** Čas, ktorý si vyžaduje spustenie úlohy, závisí od počtu zmien, ktoré treba spracovať. Veľký počet zmien trvá dlhšie. Zmluva o úrovni služieb (SLA) uvádza, že zmena používateľa v adresári služby SharePoint Online sa prejaví v aplikácii používateľského profilu o 24 hodín. 
  
[Ďalšie informácie o synchronizácii používateľského profilu v SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

