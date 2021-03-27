---
title: Automatické prihlásenie do Microsoft Edgeu
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398744"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatické prihlásenie do Microsoft Edgeu

Microsoft Edge používa predvolené konto operačného systému na automatické prihlásenie používateľa v závislosti od konfigurácie zariadenia používateľa. 

Scenáre každého typu konfigurácie zariadenia a jeho závislého procesu prihlasovania používateľom sú popísané nižšie:

- **Zariadenie je hybridné a AAD-J:** Táto možnosť je k dispozícii vo Windowse 10, systému Windows na úrovni nadol a v príslušných serverových verziách. Používatelia sú automaticky prihlásení pomocou svojich kont v službe Azure Active Directory (AD).
- **Zariadenie je pripojené k doméne:** Táto možnosť je k dispozícii vo Windowse 10, v down-level Windowse a v príslušných serverových verziách. V predvolenom nastavení nie sú používatelia s kontami domény prihlásení automaticky. ak chcete zapnúť automatické prihlásenie pre nich, použite **politiku ConfigureOnPremisesAccountAutoSignIn.** Ak chcete povoliť automatické prihlásenie pre používateľov s kontami Azure AD, zvážte hybridné pripojenie k zariadeniam.
- Predvolené konto operačného systému je **konto Microsoft:** Táto možnosť je k dispozícii vo Windowse 10 RS3 (verzia 1709, zostava 10.0.16299) a novších verziách. Scenár sa pravdepodobne vyskytuje v podnikových zariadeniach. Ak je však predvoleným kontom operačného systému konto Microsoft, Microsoft Edge sa automaticky prihlási používateľa s kontom Microsoft.
 
 
