---
title: Zdieľanie s externými používateľmi nefunguje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691590"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Riešenie problémov s zdieľaním obsahu SharePointu s externými používateľmi

Skontrolujte, či je pre vašu organizáciu zapnutá funkcia externého zdieľania:
  
1. Prejdite na [ &amp; stránku doplnky služieb v centre spravovania služby Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)a kliknite na položku **lokality**.
    
2. Skontrolujte, či je nastavenie zapnuté. Ak je vybratá možnosť len existujúci Externí používatelia, skontrolujte, či je externý používateľ uvedený v centre spravovania pre Microsoft 365.
    
Skontrolujte, či je externé zdieľanie pre lokalitu zapnuté. Pre klasickú kolekciu lokalít:
  
1. V novom centre spravovania služby SharePoint kliknite na ľavej table na položku **lokality**.
    
2. Vyberte lokalitu alebo lokality a na páse s nástrojmi kliknite na položku **Zdieľanie**.
    
Pre tímovú lokalitu, ktorá patrí do skupiny Microsoft 365 alebo na komunikačnú lokalitu:
  
- Tieto nové typy lokalít majú rovnaké nastavenie zdieľania ako nastavenie celej organizácie, pokiaľ nastavenie pre celú organizáciu neumožňuje zdieľanie súborov pomocou prepojení, ktoré nevyžadujú prihlásenie. V tomto prípade lokality povoľujú zdieľanie s novými a existujúcimi externými používateľmi, ktorí sa prihlásia. Ak chcete zmeniť nastavenie pre konkrétne lokality, použite nové centrum spravovania služby SharePoint alebo prostredie PowerShell. [Ďalšie informácie](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> Nastavenie externého zdieľania pre ľubovoľnú lokalitu môže byť reštriktívnejšie ako nastavenie celej organizácie, ale nie viac tolerantné ako nastavenie celej organizácie. 
  

