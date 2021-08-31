---
title: Problémy pri prihlasovaní do Microsoft 365 aplikácií
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
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744661"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problémy s prihlásením do Aplikácie Microsoft 365

Poznámka: Ak používate staršiu verziu balíka Windows (napríklad Windows 7 SP1, Windows Server 2008 R2), na [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) povolenie protokolu TLS 1.2 ako predvoleného použite jednoduchú opravu. Ďalšie informácie nájdete v téme Aktualizácia na povolenie [TLS 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ako predvolených zabezpečených protokolov vo WinHTTP v Windows.

Ak chcete opraviť problémy s prihlásením Microsoft 365 aplikáciami, vyskúšajte v vplyvnení počítača tieto možnosti:  

- Ďalšie Windows nájdete [Recommendations riešení bežných problémov s prihlásením](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Pre Mac si [pozrite časť Nie je možné prihlásiť sa do Office 2016 pre Mac aplikácie](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Tip** Na zariadeniach s Windowsom pre vás môžeme diagnostikovať a automaticky opraviť niekoľko bežných problémov s prihlasovaním na do balíka Office. Stiahnite a spustite asistenta **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)**, aby ste mohli používať náš automatický nástroj.

**Poznámka:** Na riešenie problémov s prihlásením alebo aktiváciou sa neodporúča vypnúť moderné overovanie (ADAL) alebo správu webového konta (WAM). Ak sa chyby vyskytnú počas pripájania k Microsoft 365 pomocou Office 2013, uistite sa, že pre klienta Office moderné overovanie. [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Konkrétne akcie na riešenie problémov nájdete v týchto téme:

[Problémy s pripojením sa pri prihlasovaní po aktualizácii na Office 2016, zostava 16.0.7967 v Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Nemôžete sa prihlásiť do konta vašej organizácie, ako je napríklad Office 365, Azure alebo Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Riešenie problémov s aplikáciami, ktoré nie sú prehliadačmi, do služieb Office 365, Azure alebo Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Opakovane výzva na zadanie poverení v Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)