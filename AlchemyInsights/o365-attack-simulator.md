---
title: 2681 Útok Simulátor v Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506753"
---
# <a name="attack-simulator-in-microsoft-365"></a>Útok Simulátor v Microsoft 365

- Chýba vám Simulátor útoku? Simulátor útoku vyžaduje **rozšírený plán ochrany pred hrozbami služieb Office 365 2 (plán ATP 2)** alebo **Office 365 Enterprise E5**. Simulátor Útok **nie** je súčasťou rozšíreného plánu ochrany pred hrozbami služieb Office 365 1 (plán ATP 1), office 365 Enterprise E3 ani v žiadnom prípade v aplikáciách Microsoft 365 pre podnikové predplatné.

- Konto, ktoré používate na spustenie simulovaných útokov, vyžaduje povolenia globálneho správcu alebo správcu zabezpečenia a viacnásobné overovanie (MFA). Ďalšie informácie o požiadavkách attack simulator nájdete [v tejto téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Dôležité veci vedieť o **Simulácia útoku Brute Force Password:**

  - Ak cieľový účet má MFA povolené a heslo uhádol správne, konto sa nezobrazí ako ohrozená (druhý overovací faktor bude neúplný).

  - Súbor s heslom nemôže byť väčší ako 10 MB. Použite jedno heslo na riadok a za posledné heslo v zozname zadajte prázdny riadok (návrat riadka).

- Dôležité informácie o **Spear Phishing** pripojiť simulácie:

  - Zámerne nie je možné zadať vlastnú hodnotu pre **adresu URL prihlasovacieho servera neoprávneného získavania údajov**.

  - Ak príjemca používa doplnok [Povoliť správu na](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) hlásenie správy ako neoprávnené získavanie údajov, pravdepodobne nebudete dostávať upozornenia na správu (pretože ide o simulovaný útok).

- Správy: Po dokončení simulovaného útoku môžete kliknúť na položku **Podrobnosti o útoku** a zobraziť prehľad.

- Podrobné pokyny a nové funkcie v aplikácii Attack Simulator nájdete v téme [Simulátor útoku v aplikácii Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
