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
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582790"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Riešenie problémov so zdieľaním obsahu SharePointu s externými používateľmi

Skontrolujte, či je pre vašu organizáciu zapnuté externé zdieľanie:
  
1. Prejdite na stránku Doplnky služby v Centre spravovania služby [Microsoft &amp; 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)a kliknite na položku **Lokality**.
    
2. Skontrolujte, či je nastavenie zapnuté. Ak je vybratá možnosť "Iba existujúci externí používatelia", uistite sa, že externý používateľ je uvedený v Centre spravovania služby Microsoft 365.
    
Skontrolujte, či je externé zdieľanie zapnuté pre lokalitu. Pre klasickú kolekciu lokalít:
  
1. V novom Centre spravovania služby SharePoint kliknite na ľavej table na položku **Lokality**.
    
2. Vyberte lokalitu alebo lokality a na páse s nástrojmi kliknite na položku **Zdieľanie**.
    
Pre tímovú lokalitu, ktorá patrí do skupiny Microsoft 365 alebo komunikačnej lokality:
  
- Tieto nové typy lokalít majú rovnaké nastavenie zdieľania ako nastavenie celej organizácie, pokiaľ nastavenie pre celú organizáciu nepovoľuje zdieľanie súborov pomocou prepojení, ktoré nevyžadujú prihlásenie. V tomto prípade lokality umožňujú zdieľanie s novými a existujúcimi externými používateľmi, ktorí sa prihlasujú. Ak chcete zmeniť nastavenie pre konkrétne lokality, použite nové Centrum spravovania služby SharePoint alebo Prostredie PowerShell. [Ďalšie informácie](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> Nastavenie externého zdieľania pre ľubovoľnú lokalitu môže byť prísnejšie ako nastavenie celej organizácie, ale nie tolerantnejšie ako nastavenie platné v celej organizácii. 
  

