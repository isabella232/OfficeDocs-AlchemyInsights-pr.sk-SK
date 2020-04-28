---
title: Zdieľanie s externými používateľmi nefunguje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913017"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Riešenie problémov s zdieľaním obsahu služby SharePoint s externými používateľmi

Presvedčte sa, či je pre vašu organizáciu zapnuté externé zdieľanie:
  
1. Prejdite na [stránku služby &amp; doplnky Microsoft 365 admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)a kliknite na tlačidlo **lokality**.
    
2. Presvedčte sa, či je nastavenie zapnuté "zapnuté". Ak je vybratá možnosť "iba existujúcich externých používateľov", uistite sa, že externý používateľ je uvedený v Microsoft 365 admin Center.
    
Skontrolujte, či je pre lokalitu zapnuté externé zdieľanie. Pre klasickú kolekciu lokalít:
  
1. V novom SharePoint admin Center, na ľavej table kliknite na položku **lokality**.
    
2. Vyberte lokalitu alebo lokality a na páse s nástrojmi kliknite na položku **Zdieľanie**.
    
Pre tímovú lokalitu, ktorá patrí do skupiny Microsoft 365 alebo na komunikačnú lokalitu:
  
- Tieto nové typy lokalít majú rovnaké nastavenie zdieľania ako nastavenie pre celú organizáciu, pokiaľ nastavenie pre celú organizáciu umožňuje zdieľanie súborov pomocou prepojení, ktoré nevyžadujú prihlásenie. V tomto prípade lokality umožňujú zdieľanie s novými a existujúcimi externými používateľmi, ktorí sa prihlasujú. Ak chcete zmeniť nastavenie pre konkrétne lokality, použite nové centrum spravovania služby SharePoint alebo PowerShell. [Ďalšie informácie](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> Nastavenie externého zdieľania pre ľubovoľnú lokalitu môže byť obmedzujúcejšie ako nastavenie pre celú organizáciu, ale nie viac tolerantnejšie ako nastavenie celej organizácie. 
  

