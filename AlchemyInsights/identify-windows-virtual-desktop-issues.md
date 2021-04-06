---
title: Identifikácia problémov týkajúcich sa virtuálnej pracovnej plochy Windowsu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596040"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identifikácia problémov týkajúcich sa virtuálnej pracovnej plochy Windowsu

Diagnostika virtuálnej pracovnej plochy systému Windows používa iba jednu rutinu typu cmdlet prostredia PowerShell, no obsahuje mnoho voliteľných parametrov, ktoré vám pomôžu určiť a určiť problémy. Začíname: 

1. Stiahnite a importujte modul Windows Virtual Desktop PowerShell. Podrobnosti nájdete v téme [Rutiny typu cmdlet virtuálnej pracovnej plochy Windowsu pre Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Na prihlásenie do konta spustite nasledujúcu rutinu cmdlet:
    
    Príklad: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**POZNÁMKA:** Všetky dotazy používajúce prostredie PowerShell musia obsahovať parametre -UserName alebo -ActivityID. Informácie o možnostiach sledovania nájdete v téme [Používanie analýzy denníka pre diagnostické funkcie.](https://go.microsoft.com/fwlink/?linkid=2126847)

Ak chcete filtrovať diagnostické aktivity podľa používateľa, spustite nasledujúcu rutinu cmdlet:

Príklad: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

K dispozícii je zoznam filtrov, pomocou ktorých môžete diagnostikovať problémy. Ďalšie informácie o diagnostike problémov nájdete v téme Identifikácia a [diagnostika problémov virtuálnej pracovnej plochy Windowsu.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Ďalšie informácie o bežných chybách nájdete v [téme Bežné chyby ako šucháky](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
