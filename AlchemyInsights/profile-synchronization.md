---
title: Synchronizácia profilu
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768128"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kedy sa môj profil zmení na synchronizáciu s aplikáciou používateľského profilu služby SharePoint?

SharePoint Online používa Active Directory import časovač prácu (AD Import) importovať používateľov a skupín do aplikácie používateľského profilu. 
  
1. AD Import synchronizuje zmeny z lokality SharePoint Online Directory Store do aplikácie používateľského profilu. Tieto zmeny sa spracúvajú v dávkach.
    
2. Úloha časovača sa spustí, kým sa zmeny nesynchronizujú.
    
> [!NOTE]
> Čas potrebný na spustenie úlohy závisí od počtu zmien, ktoré sa majú spracovať. Veľké množstvo zmien trvá dlhšie. Zmluva o úrovni služieb (SLA) uvádza, že zmena používateľa v adresári SharePoint Online sa prejaví v aplikácii používateľského profilu v 24 hodín. 
  
[Ďalšie informácie o synchronizácii používateľského profilu v SharePointe Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

