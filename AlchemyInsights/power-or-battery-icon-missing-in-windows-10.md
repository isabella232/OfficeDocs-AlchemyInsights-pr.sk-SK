---
title: Ikona napájania alebo batérie chýba vo Windowse 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 82d41844de1eafdf7e0cc38f91416f3b71868e3d5d1b3eb8be0f10abd701ddc8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973362"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Ikona napájania alebo batérie chýba vo Windowse 10

Ak vaše zariadenie s Windowsom 10 obsahuje batériu (napríklad notebook alebo tablet alebo počítač pripojený cez USB k záložnému zdroju UPS), na paneli úloh v blízkosti hodín sa zvyčajne zobrazuje ikona napájania alebo batérie, napríklad:

![Ikona batérie](media/battery-icon.png)

Ak sa táto ikona nezobrazuje, môže byť skrytá:

1. Prejdite na položky **[Nastavenia > Prispôsobenie > Panel úloh](ms-settings:taskbar?activationSource=GetHelp)**.

2. V časti Oblasť oznámení kliknite na položku **Vyberte ikony, ktoré sa budú zobrazovať na paneli úloh**.

3. Potom v zozname vyhľadajte položku **Napájanie** a prepnite jej nastavenie na možnosť **Zapnuté**.

    ![Zobrazenie ikony napájania na paneli úloh](media/power-icon-on.png)

**Riešenie problémov**

Ak ste postupovali podľa uvedených pokynov a prepínač **Napájanie** je sivý alebo sa nezobrazuje, do vyhľadávacieho poľa na paneli úloh napíšte výraz **správca zariadení** a potom v zozname výsledkov vyberte položku **Správca zariadení**. V časti **Batérie** kliknite pravým tlačidlom myši na batériu zariadenia, kliknite na položku **Zakázať** a potom na položku **Áno**. Počkajte niekoľko sekúnd, kliknite pravým tlačidlom myši na batériu a kliknite na položku **Povoliť**. Potom reštartujte zariadenie.

Ak ste postupovali podľa uvedených pokynov, ale ikona batérie sa na paneli úloh nezobrazuje, do vyhľadávacieho poľa na paneli úloh napíšte výraz **správca úloh** a potom v zozname výsledkov kliknite na položku **Správca úloh**. Na karte **Procesy** v stĺpci časti **Názov** kliknite pravým tlačidlom myši na položku **Prieskumník** a potom kliknite na položku **Reštartovať**.
