---
title: Endpoint DLP not deployed to user's device
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731867"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Endpoint DLP not deployed to user's device

Ak sa nastavenie Ochrany pred stratou údajov (DLP) koncového bodu ešte v zariadení používateľa použilo, potvrďte, že spĺňate tieto požiadavky:

- Windows 10 je v zariadení nainštalovaná zostava x64 1809 alebo novšia.
- Je nainštalovaný anti malware client verzie 4.18.2009.7 alebo novšej.
- Zariadenie je **jedným z** týchto zariadení:
    
    - Azure Active Directory (Azure AD)
    - Hybridný Azure AD pripojený
    - Zaregistrované AAD

- Ak chcete uplatniť akcie politiky, uistite sa, Chromium máte v koncovom zariadení nainštalovaný prehliadač Microsoft Chromium Edge.

Ďalšie požiadavky na nasadenie politiky DLP koncového bodu nájdete v téme Začíname s [ochrane pred stratou údajov koncových bodov.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)