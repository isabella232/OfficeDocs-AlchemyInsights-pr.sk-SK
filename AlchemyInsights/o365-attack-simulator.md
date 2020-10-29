---
title: Simulátor útoku 2681 v Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801566"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulátor útoku v programe Microsoft 365

- Chýba vám simulátor útoku? Simulátor útoku vyžaduje **program Microsoft Defender pre office 365 Plan 2 (ATP Plan 2)** alebo **Office 365 Enterprise E5** . Simulátor útoku **nie** je zahrnutý v programe Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3 ani v ktorejkoľvek aplikácii Microsoft 365 for Business.

- Konto, ktoré používate na spustenie simulovaných útokov, vyžaduje globálny správca alebo povolenia správcu zabezpečenia a viacnásobné overovanie (MFA). Ďalšie informácie o požiadavkách útoku simulátora nájdete v [tejto téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Dôležité informácie o simuláciách útoku **brutálnych síl na heslo** :

  - Ak má cieľové konto zapnuté MFA a heslo sa nesprávne zobrazilo, konto sa nebude zobrazovať ako ohrozené (druhý overovací faktor bude neúplný).

  - Súbor s heslom nemôže byť väčší ako 10 MB. Použite jedno heslo na jeden riadka a do zoznamu pridajte prázdny (znak konca riadka).

- Dôležité informácie o tom, ako **neoprávnené získavanie údajov** o službe kopije:

  - Návrhom nie je možné poskytnúť vlastnú hodnotu pre **URL adresu prihlasovacieho servera pre neoprávnené získavanie údajov** .

  - Ak príjemca použije [doplnok povoliť správu zostavy](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) na nahlásenie správy ako neoprávneného získavania údajov, možno nebudete dostávať upozornenia na správu (pretože ide o simulovaný útok).

- Zostavy: po dokončení simulovaného útoku môžete kliknutím na položku Podrobnosti o **útoku** Zobraziť zostavu.

- Podrobné pokyny a nové funkcie v simulátore útoku nájdete [v téme simulátor útoku v Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
