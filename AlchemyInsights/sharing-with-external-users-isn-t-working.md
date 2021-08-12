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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910381"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Riešenie problémov so zdieľaním obsahu SharePointu s externými používateľmi

Uistite sa, že je vo vašej organizácii zapnuté externé zdieľanie:
  
1. Prejdite na [stránku Doplnky služieb v Centre &amp; spravovania služby Microsoft 365 a](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)kliknite na položku **Lokality.**
    
2. Uistite sa, že nastavenie je zapnuté. Ak je vybratá možnosť Iba existujúci externí používatelia, uistite sa, že externý používateľ je uvedený v Centre spravovania služby Microsoft 365.
    
Uistite sa, že je pre lokalitu zapnuté externé zdieľanie. Pre klasickú kolekciu lokalít:
  
1. V novom Centre spravovania služby SharePoint kliknite na ľavej table na položku **Lokality**.
    
2. Vyberte lokalitu alebo lokality a na páse s nástrojmi kliknite na položku **Zdieľanie**.
    
Pre tímovú lokalitu, ktorá patrí do skupiny služby Microsoft 365 alebo lokality na komunikáciu:
  
- Tieto nové typy lokalít majú rovnaké nastavenie zdieľania ako nastavenie pre celú organizáciu, pokiaľ nastavenie celej organizácie nepožaduje zdieľanie súborov pomocou prepojení, ktoré nevyžadujú prihlásenie. V tomto prípade lokality umožňujú zdieľanie s novými a existujúcimi externými používateľmi, ktorí sa prihlásia. Ak chcete zmeniť nastavenie pre konkrétne lokality, použite nové Centrum spravovania služby SharePoint alebo prostredie PowerShell. [Ďalšie informácie](https://go.microsoft.com/fwlink/?linkid=871863)
    
> [!NOTE]
> Nastavenie externého zdieľania pre ľubovoľnú lokalitu môže byť prísnejšie ako nastavenie v celej organizácii, ale nemusí byť viac obmedzujúce ako nastavenie v celej organizácii. 
  

