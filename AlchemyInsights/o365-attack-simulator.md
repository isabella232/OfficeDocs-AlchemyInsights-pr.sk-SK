---
title: 2681 útoku simulátor v Microsoft 365
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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713481"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulátor útoku v Microsoft 365

- Ste chýbajúce útoku simulátor? Attack Simulator vyžaduje **office 365 pokročilé ohrozenia ochrany plán 2 (ATP Plan 2)** alebo **Office 365 Enterprise E5**. Attack Simulator **nie** je zahrnutá v balíku Office 365 pokročilé ohrozenia ochrany plán 1 (ATP Plan 1), Office 365 Enterprise E3 alebo akékoľvek Microsoft 365 aplikácie pre podnikové predplatné.

- Konto, ktoré používate na spustenie simulovaných útokov vyžaduje globálny správca alebo povolenia správcu zabezpečenia a viacnásobné overovanie (MFA). Ďalšie informácie o požiadavkách na simulátore útoku nájdete [v tejto téme](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Dôležité veci vedieť o **hrubou silou heslo** útoku simulácie:

  - Ak cieľový účet má MFA povolené a heslo bolo uhádnuť správne, účet nebude zobrazovať ako ohrozená (druhý overovací faktor bude neúplné).

  - Súbor s heslom nemôže byť väčší ako 10 MB. Použite jedno heslo na riadok a po poslednom hesle v zozname zahrňte prázdny riadok (návrat vozíka).

- Dôležité veci vedieť o **Spear phishing** priložiť simulácie:

  - Podľa návrhu nemôžete poskytnúť vlastnú hodnotu **adresy URL prihlasovacieho servera pre neoprávnené získavanie údajov**.

  - Ak príjemca používa povoliť správu správa [Add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) hlásiť správy ako phishing, nemusí dostávať upozornenia na správu (pretože to je simulovaný útok).

- Prehľady: po dokončení simulovaného útoku môžete kliknutím na položku **Podrobnosti o útoku** Zobraziť zostavu.

- Podrobné pokyny a nové funkcie v útoku simulátor, pozri [útoku simulátor v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
