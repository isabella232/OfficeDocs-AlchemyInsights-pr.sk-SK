---
title: Teams sa nespustí
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813358"
---
# <a name="teams-doesnt-launch"></a>Teams sa nespustí

Ak sa pokúsite otvoriť Microsoft Teams sa nespustí, vyskúšajte tento postup:

1. Prejdite na **lokalitu %appdata%\Microsoft\Teams.**
1. Odstráňte obsah priečinka.
1. Reštartujte počítač a skúste spustiť Teams.

Pravdepodobne bude potrebné znova nainštalovať Teams. Preinštalovanie:

1. Odinštalujte Teams pomocou ovládacieho panela.
1. Prejdite na **lokalitu %appdata%\Microsoft\Teams\Application Cache**.
1. Odstráňte obsah priečinka.
1. Prejdite na **položku %appdata%\Microsoft\teams\Cache**.
1. Odstráňte obsah priečinka.
1. Reštartujte počítač a potom stiahnite a nainštalujte Teams.

Ak chcete v nájomníkovi spustiť diagnostiku pre konkrétneho používateľa, ktorý sa nemôže prihlásiť, spustite nové vyhľadávanie s kľúčovým slovom **TeamsUserUnableToSignIn** a postupujte podľa pokynov.