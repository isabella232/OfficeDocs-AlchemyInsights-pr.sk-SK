---
title: Povoľte používateľovi synchronizovať osobné konto s pracovným kontom v Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813406"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Povoľte používateľovi synchronizovať osobné konto s pracovným kontom v Microsoft Edge

Skontrolujte, či spĺňate tieto kritériá:

- Enterprise State Roaming je povolený v Centre spravovania Azure Active Directory, ktoré vyžaduje predplatné na Azure Active Directory Premium alebo Enterprise Mobility + Security (EMS). Ďalšie informácie nájdete v téme [Zapnutie podnikového roamingu v Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Spĺňajú jedno alebo obe nasledujúce kritériá:
    - Nájomník má zapnutú službu Azure Information Protection. Podrobnosti nájdete v téme [Aktivácia ochrany Azure Rights Management v Centrum spravovania služby Microsoft 365.](/azure/information-protection/activate-office365)
    - Funkcia Azure Active Directory Enterprise State Roaming (ESR) je povolená pre ľubovoľného používateľa alebo nájomníka. Ďalšie informácie nájdete v téme [Čo je roaming podnikového stavu?](/azure/active-directory/devices/enterprise-state-roaming-overview)

Ak sú AIP aj ESR vypnuté, chybové hlásenie informuje používateľov, že synchronizácia nie je k dispozícii pre ich kontá.
