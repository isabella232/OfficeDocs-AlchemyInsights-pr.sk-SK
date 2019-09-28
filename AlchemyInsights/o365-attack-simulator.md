---
title: 2681 útoku simulátor v balíku Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305346"
---
# <a name="attack-simulator-in-office-365"></a>Simulátor útoku v balíku Office 365

- Ste chýbajúce útoku simulátor? Attack Simulator vyžaduje **office 365 pokročilé ohrozenia ochrany plán 2 (ATP Plan 2)** alebo **Office 365 Enterprise E5**. Útok simulátor **nie** je zahrnutá v balíku Office 365 pokročilé ohrozenia ochrany plán 1 (ATP Plan 1), Office 365 Enterprise E3 alebo akékoľvek Office 365 Business predplatné.

- Konto, ktoré používate na spustenie simulovaných útokov vyžaduje globálny správca alebo povolenia správcu zabezpečenia a viacnásobné overovanie (MFA). Ďalšie informácie o požiadavkách na simulátore útoku nájdete [v tejto téme](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Dôležité veci vedieť o **hrubou silou heslo** útoku simulácie:

  - Ak cieľový účet má MFA povolené a heslo bolo uhádnuť správne, účet nebude zobrazovať ako ohrozená (druhý overovací faktor bude neúplné).

  - Súbor s heslom nemôže byť väčší ako 10 MB. Použite jedno heslo na riadok a po poslednom hesle v zozname zahrňte prázdny riadok (návrat vozíka).

- Dôležité veci vedieť o **Spear phishing** priložiť simulácie:

  - Podľa návrhu nemôžete poskytnúť vlastnú hodnotu **adresy URL prihlasovacieho servera pre neoprávnené získavanie údajov**.

  - Ak príjemca používa povoliť správu správa [Add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) hlásiť správy ako phishing, nemusí dostávať upozornenia na správu (pretože to je simulovaný útok).

- Prehľady: po dokončení simulovaného útoku môžete kliknutím na položku **Podrobnosti o útoku** Zobraziť zostavu.

- Podrobné pokyny a nové funkcie v útoku simulátor, pozri [Attack Simulator v balíku Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
