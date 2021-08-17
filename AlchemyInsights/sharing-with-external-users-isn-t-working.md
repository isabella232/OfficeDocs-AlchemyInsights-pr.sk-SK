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
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304384"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Riešenie problémov so SharePoint obsahom s externými používateľmi

Uistite sa, že máte v organizácii zapnuté externé zdieľanie:
  
1. Prejdite na [stránku Doplnky služieb v &amp; prvej Centrum spravovania služby Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)a kliknite na položku **Lokality**.
    
2. Uistite sa, že nastavenie je zapnuté. Ak je vybratá možnosť Iba existujúci externí používatelia, uistite sa, že externý používateľ je uvedený v zozname Centrum spravovania služby Microsoft 365.
    
Uistite sa, že je pre lokalitu zapnuté externé zdieľanie. Pre klasickú kolekciu lokalít:
  
1. V novom centre SharePoint kliknite na ľavej table na položku **Lokality**.
    
2. Vyberte lokalitu alebo lokality a na páse s nástrojmi kliknite na položku **Zdieľanie**.
    
Pre tímovú lokalitu, ktorá patrí do Microsoft 365 alebo komunikačnej lokality:
  
- Tieto nové typy lokalít majú rovnaké nastavenie zdieľania ako nastavenie pre celú organizáciu, pokiaľ nastavenie celej organizácie nepožaduje zdieľanie súborov pomocou prepojení, ktoré nevyžadujú prihlásenie. V tomto prípade lokality umožňujú zdieľanie s novými a existujúcimi externými používateľmi, ktorí sa prihlásia. Ak chcete zmeniť nastavenie pre konkrétne lokality, použite nové centrum spravovania SharePoint alebo prostredie PowerShell. [Ďalšie informácie](https://go.microsoft.com/fwlink/?linkid=871863)
    
**Poznámka:** Nastavenie externého zdieľania pre ľubovoľnú lokalitu môže byť prísnejšie ako nastavenie v celej organizácii, ale nemôže byť viac obmedzujúce ako nastavenie v celej organizácii. 
  

