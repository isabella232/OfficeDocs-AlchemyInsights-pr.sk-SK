---
title: Podmienený prístup pomocou Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505009"
---
# <a name="conditional-access-with-intune"></a>Podmienený prístup pomocou Intune

Použitie **podmieneného prístupu** s Intune vyžaduje 3 kroky: 
  
- Vytvorte **politiku podmieneného prístupu** , ktorá definuje, aké prostriedky sú chránené, a aké podmienky je potrebné splniť na prístup k týmto prostriedkom. Zariadenie musí byť napríklad kompatibilné pred prístupom do podnikového e-mailu. 
    
- Vytvorenie **politiky súladu** na definovanie nastavení, ktoré musia byť splnené pred tým, ako sa zariadenie považuje za vyhovujúce. Zariadenie musí mať napríklad PIN aspoň 6 číslic predtým, ako sa považuje za vyhovujúce. 
    
- Zabezpečenie **politík súladu** a **politiky podmieneného prístupu** sú zacielené na želané skupiny používateľov. To môže vyžadovať vytvorenie konkrétnych skupín používateľov v Azure Active Directory. 
    
Čítajte viac:
  
- [Osvedčené postupy podmieneného prístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Začíname s podmieneným prístupom](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

