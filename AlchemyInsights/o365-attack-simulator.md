---
title: 2681 Attack Simulator v Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325086"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator in Microsoft 365

- Chýba vám Attack Simulator? Attack Simulator vyžaduje **microsoft Defender pre Office 365 Plan 2** alebo Office 365 Enterprise **E5.** Attack Simulator nie **je** súčasťou programu Microsoft Defender pre Office 365 Plan 1, Office 365 Enterprise E3 ani žiadne Aplikácie Microsoft 365 pre podnikateľov predplatné.

- Konto, ktoré používate na spustenie simulovaných útokov, vyžaduje povolenia globálneho správcu alebo správcu zabezpečenia a viacfaktorové overovanie (MFA). Ďalšie informácie o požiadavkách na Attack Simulator nájdete v [tejto téme.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Dôležité informácie o simuláciách **útokov Brute Force Password:**

  - Ak má cieľové konto zapnuté viacfaktorové overovanie a heslo bolo správne uhádnuť, konto sa nebude zobrazovať ako zneužiné (druhý overovací faktor bude neúplný).

  - Súbor hesiel nemôže byť väčší ako 10 MB. Použite jedno heslo na jeden riadok a za posledné heslo v zozname uveďte prázdny riadok (koniec riadka).

- Dôležité veci, ktoré by ste mali vedieť o **Tomsi Phishingu, pripájajú** simulácie:

  - Nie je možné poskytnúť vlastnú hodnotu prihlasovacej adresy servera neoprávneného získavania **údajov na základe** návrhu.

  - Ak príjemca použije [](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) doplnok Povoliť správu správu na nahlásenie neoprávneného získavania údajov, je možné, že sa na správu nebudú prijímať upozornenia (pretože ide o simulovaný útok).

- Zostavy: Po dokončení simulovaného útoku môžete kliknutím na položku **Podrobnosti o útoke** zobraziť zostavu.

- Podrobné pokyny a nové funkcie v attack Simulatore nájdete v téme [Attack Simulator v Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
