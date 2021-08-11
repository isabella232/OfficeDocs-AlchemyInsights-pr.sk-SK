---
title: Testovanie konfigurácie IRM pre nové možnosti OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812446"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testovanie konfigurácie IRM pre nové možnosti OME

Ak chcete overiť, či je váš Microsoft 365 nájomník nakonfigurovaný na používanie nových možností OME, spustite po pripojení k [Exchange Online PowerShell nasledujúce rutiny](/powershell/exchange/exchange-online-powershell)cmdlet:


1. Skontrolujte konfiguráciu správy prístupových práv k informáciám nájomníka spustením služby `Get-IRMConfiguration` . Skontrolujte, či sú tieto hodnoty nastavené na **hodnotu True:**
    
    **InternalLicensingEnabled**
    
    **ExternáLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Pomocou domény, adresy odosielateľa a príjemcu spustite `Test-IRMConfiguration` . Ak test neprejde, preskúmajte konfiguráciu SPRÁVY prístupových práv k informáciám.

Ďalšie informácie o overení konfigurácie SPRÁVY prístupových práv k informáciám nájdete v téme [Overenie novej konfigurácie OME v Exchange Online PowerShell.](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)