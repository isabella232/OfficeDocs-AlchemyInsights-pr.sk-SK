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
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801784"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kedy sa zmení môj profil na synchronizáciu s aplikáciou používateľských profilov SharePointu?

V SharePointe Online sa na importovanie používateľov a skupín do aplikácie používateľského profilu používa úloha časovača importu služby Active Directory (Import reklamy). 
  
1. Importovanie reklám synchronizuje zmeny z adresárového obchodu SharePoint Online do aplikácie používateľského profilu. Tieto zmeny sa spracúvajú v dávkach.
    
2. Úloha časovača sa spustí, až kým sa zmeny nesynchronizujú.
    
> [!NOTE]
> Časový úsek, v ktorom sa spustí úloha, závisí od počtu zmien, ktoré sa majú spracovať. Veľký počet zmien trvá dlhšie. V zmluve o úrovni služieb (SLA) sa uvádza, že zmeny používateľa v adresári služby SharePoint Online sa prejavia v aplikácii používateľského profilu v priebehu 24 hodín. 
  
[Ďalšie informácie o synchronizácii používateľských profilov v SharePointe Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

