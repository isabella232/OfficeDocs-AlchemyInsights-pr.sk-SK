---
title: Problém s pripojením k VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885662"
---
# <a name="issue-joining-vms"></a>Problém s pripojením k VMs

Ak chcete vyriešiť problémy, ktoré sa vyskytujú pri pokuse o spojenie s VMs, vykonajte tieto kroky:

1. Skúste sa prihlásiť pomocou formátu **UPN** (napríklad "JoeUser@contoso.com") namiesto formátu **SAMAccountName** (' CONTOSO\joeuser ').
2. Skontrolujte, či ste povolili synchronizáciu hesiel v súlade s krokmi uvedenými v *príručke Začíname* .
3. Skontrolujte, či príslušné používateľské konto nie je externým kontom v nájomníkovi služby Azure AD. Externí používatelia sa nemôžu prihlásiť do spravovanej domény, pretože služby Azure AD Domain neobsahujú poverenia pre takéto používateľské kontá.
4. Ak je postihnuté používateľské konto iba v cloude, zabezpečte, aby používatelia zmenili svoje heslo po zapnutí služby Azure AD Domain Services. Tento krok spôsobuje hodnoty hash poverení vyžadované na generovanie služieb Azure AD domain.
5. Ak sa príslušné používateľské kontá synchronizujú z lokálneho adresára, overte, či je odporúčaná verzia služby Azure AD Connect nakonfigurovaná na vykonanie úplnej synchronizácie.
6. Ak problémy pretrvávajú aj po potvrdení kroku 4, spustite nasledujúce príkazy zo zariadenia na synchronizáciu:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.