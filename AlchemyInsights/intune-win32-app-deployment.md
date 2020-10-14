---
title: Intune nasadenie aplikácií Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461991"
---
# <a name="intune-win32-app-deployment"></a>Intune nasadenie aplikácií Win32

Microsoft Intune povoľuje aplikácie Win32 vrátane, ale nie výhradne, MSI a. EXE, ktorý sa má nasadiť v zariadeniach s Windowsom 10. Použitý mechanizmus nasadenia vyžaduje, aby sa v cieľovom zariadení nachádzalo rozšírenie správy služby Intune (IME). Editor IME sa automaticky nainštaluje ako výsledok zamerania skriptu prostredia PowerShell alebo nasadenia aplikácie Win32 na používateľa alebo zariadenie.

K dispozícii je tiež množina predpokladov, ktoré musia byť splnené, aby sa nasadili aplikácie Win32, ktoré zahŕňajú:

- Podporované platformy: Windows 10 version 1607 alebo novšia verzia (podnikové, Pro a vzdelávacie verzie).
- Podporovaná architektúra: x86 a x64.
- Správa zariadenia: AAD sa pripojil a automaticky zaregistroval (vrátane hybridnej domény pripojenej a skupinovej politiky automaticky zaregistrovaných).
- Formát balíka aplikácií:. súbor **intunewin**  pripravený nástrojom na [prípravu obsahu Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Obmedzenia
    - Maximálna veľkosť: 8GB.
    - Nepodporovaná architektúra: zbrane.

Ďalšie informácie týkajúce sa týchto krokov nájdete[v téme Pridanie, priradenie a sledovanie aplikácie Win32 v službe Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add).

Podrobnosti o riešení problémov s nasadením aplikácií vo Windowse vrátane aplikácií Win32 je možné preskúmať v týchto dokumentoch

- [Riešenie problémov s inštaláciou aplikácie](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Riešenie problémov s aplikáciami Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)