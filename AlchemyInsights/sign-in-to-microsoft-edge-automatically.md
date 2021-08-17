---
title: Automatické prihlásenie Microsoft Edge prihlásení
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050709"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatické prihlásenie Microsoft Edge prihlásení

Microsoft Edge používa predvolené konto operačného systému na automatické prihlásenie používateľa v závislosti od konfigurácie zariadenia používateľa. 

Scenáre každého typu konfigurácie zariadenia a jeho závislého procesu prihlasovania používateľom sú popísané nižšie:

- **Zariadenie je hybridné a AAD-J:** Táto možnosť je k dispozícii Windows 10 serverových verziách, Windows úrovni servera a príslušných verziách servera. Používatelia sú automaticky prihlásení pomocou svojich Azure Active Directory (AD).
- **Zariadenie je pripojené k doméne:** Táto možnosť je k dispozícii Windows 10 pre všetky verzie servera, Windows úrovni servera a príslušné verzie servera. V predvolenom nastavení nie sú používatelia s kontami domény prihlásení automaticky. ak chcete zapnúť automatické prihlásenie pre nich, použite **politiku ConfigureOnPremisesAccountAutoSignIn.** Ak chcete povoliť automatické prihlásenie pre používateľov s kontami Azure AD, zvážte hybridné pripojenie k zariadeniam.
- Predvolené konto operačného systému je **konto Microsoft:** Táto možnosť je k dispozícii v systéme Windows 10 RS3 (verzia 1709, zostava 10.0.16299) a v novších verziách. Scenár sa pravdepodobne vyskytuje v podnikových zariadeniach. Ak je však predvoleným kontom operačného systému konto Microsoft, Microsoft Edge automaticky prihlási používateľa s kontom Microsoft.
 
 
