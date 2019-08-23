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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554348"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Keď môj profil zmeny synchronizovať SharePoint používateľa profil aplikácie?

SharePoint Online používa Active Directory Import časovača (AD Import) importovať používateľov a skupín do aplikácie používateľského profilu. 
  
1. AD Import synchronizuje zmeny z lokality SharePoint Online adresár Store aplikácie používateľského profilu. Tieto zmeny sú spracované v dávkach.
    
2. Úloha časovača beží, kým sa zmeny nesynchronizujú.
    
> [!NOTE]
> Čase, keď sa má spustiť úloha závisí od počtu zmien spracovať. Veľký počet zmien trvá dlhšie. Service Level Agreement (SLA) uvádza, že zmena používateľa v adresári služby SharePoint Online sa prejaví v aplikácii používateľského profilu v 24 hodín. 
  
[Viac informácií o synchronizácia používateľského profilu SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

