---
title: Automaticky sa prihláste do prehliadača Microsoft Edge
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678815"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automaticky sa prihláste do prehliadača Microsoft Edge

Microsoft Edge používa predvolené konto operačného systému na automatické prihlásenie používateľa podľa toho, ako je zariadenie používateľa nakonfigurované. 

Scenáre jednotlivých typov konfigurácie zariadenia a jeho prihlasovacieho procesu závislého používateľa sú popísané nižšie:

1. **Zariadenie je hybridné/AAD-J**: Táto možnosť je k dispozícii vo Windowse 10, Windowse nadol a v zodpovedajúcich verziách servera. Používatelia sú automaticky prihlásení pomocou svojich kont služby Azure Active Directory (AD).
2. **Zariadenie je pripojené k doméne**: Táto možnosť je k dispozícii vo Windowse 10, systéme Windowse na úrovni nižšie a v zodpovedajúcich verziách servera. Používatelia s kontom domény sa predvolene nepodpisujú automaticky. Ak chcete povoliť automatické prihlasovanie, použite politiku **ConfigureOnPremisesAccountAutoSignIn** . Ak chcete povoliť automatické prihlasovanie pre používateľov s kontom Azure AD, zvážte hybridné pripojenie k svojim zariadeniam.
3. **Predvoleným kontom operačného systému je konto Microsoft**: Táto možnosť je k dispozícii vo Windowse 10 RS3 (verzia 1709, Zostava 10.0.16299) a v novších verziách. V podnikových zariadeniach nie je pravdepodobné, že sa vyskytne scenár. Ak je však predvoleným kontom operačného systému konto Microsoft, Microsoft Edge sa automaticky prihlási používateľovi s kontom Microsoft.
 
 
