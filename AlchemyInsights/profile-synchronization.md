---
title: Synchronizácie profilu
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371999"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Keď môj profil zmeny synchronizovať SharePoint používateľa profil aplikácie?

SharePoint Online používa Active Directory Import časovača (AD Import) importovať používateľov a skupín do aplikácie používateľského profilu. 
  
1. AD Import synchronizuje zmeny z lokality SharePoint Online adresár Store aplikácie používateľského profilu. Tieto zmeny sú spracované v dávkach.
    
2. Úloha časovača beží, kým sa zmeny nesynchronizujú.
    
> [!NOTE]
> Čase, keď sa má spustiť úloha závisí od počtu zmien spracovať. Veľký počet zmien trvá dlhšie. Service Level Agreement (SLA) uvádza, že zmena používateľa v adresári služby SharePoint Online sa prejaví v aplikácii používateľského profilu v 24 hodín. 
  
[Viac informácií o synchronizácia používateľského profilu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

