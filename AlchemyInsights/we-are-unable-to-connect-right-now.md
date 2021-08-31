---
title: Problém s aktiváciou – nepodarilo sa nám pripojiť
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744610"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Oprava Microsoft 365 hlásení "Nepodarilo sa pripojiť"

Poznámka: Ak používate staršiu verziu balíka Windows (napríklad Windows 7 SP1, Windows Server 2008 R2), na [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) povolenie protokolu TLS 1.2 ako predvoleného použite jednoduchú opravu. Ďalšie informácie nájdete v téme Aktualizácia na povolenie [TLS 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ako predvolených zabezpečených protokolov vo WinHTTP Windows.

Ak sa zobrazí toto hlásenie, skúste toto:

1. Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy a overte, či neblokujú prístup na internet k Microsoft 365 aplikáciám. Pozrite [si časť URL adresy a rozsahy IP adries od spoločnosti Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Prejdite do **ponuky**  >  **Spustiť spustenie** a zadajte reťazec **services.msc.** Skontrolujte, či sú spustené všetky tieto služby:
    - Automatické nastavenie zariadení pripojených k sieti
    - Služba so zoznamom sietí
    - Informovanosť o sieťovom umiestnení
    - Windows Denník udalostí

Ak niektorá z týchto služieb nie je spustená, skúste ju spustiť. Ak máte problém so spustením služby, spustite nasledujúci príkaz otvorením príkazového riadka s zvýšenými povoleniami:

**sfc /scannow**

Po dokončení tohto príkazu reštartujte počítač.

Podrobné informácie nájdete v časti [Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr" pri aktivácii Office z Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).