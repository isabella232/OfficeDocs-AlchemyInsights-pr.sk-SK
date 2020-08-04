---
title: Používanie aplikácie TeamViewer na vzdialenú správu zariadení Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555749"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Používanie aplikácie TeamViewer na vzdialenú správu zariadení Intune

Zariadenia spravované aplikáciou Intune je možné spravovať na diaľku pomocou [aplikácie TeamViewer](https://www.teamviewer.com/).

Ak chcete spravovať aplikáciu Intune pomocou aplikácie TeamViewer, postupujte takto: 

Začnite získaním poverení z aplikácie TeamViewer na nastavenie konektora TeamViewer v programe Intune. To umožňuje správcovi zadať poverenia v používateľskom rozhraní konektora TeamViewer v časti Zariadenia, čo je jednorázová operácia na vytvorenie prepojenia medzi intune a službou TeamViewer.

**Časť 1: Spustenie relácie so vzdialeným zariadením**

1. V **časti Všetky**zariadenia vyberte zariadenie, s ktorými chcete spustiť vzdialenú reláciu.
2. Od **... 3/4e**vyberte **Nová relácia pomoci na diaľku**.
3. Ak chcete **potvrdiť,** že chcete vytvoriť vzdialenú reláciu, vyberte možnosť Áno.
    Po tom, ako služba TeamViewer potvrdí žiadosť "Inicializácia novej vzdialenej **Start remote assistance** relácie", sa na table Prehľad (alebo Essentials) zariadenia zobrazí možnosť Spustiť pomoc na diaľku. Výberom **položky Zobraziť ďalšie** rozbaľte tablu a zobrazte stav Pomoci na diaľku.
4. Výberom **položky Spustiť vzdialenú** reláciu spustite reláciu na strane správcu.
5. Vyberte, či chcete stiahnuť binárny súbor aplikácie TeamViewer (Windows) a vyberte položku **Spustiť**.<br/>
    **Upozornenie:** Môžete ignorovať ľubovoľnú stránku webového prehľadávača otvorenú na webovej lokalite aplikácie TeamViewer.

6. Potvrďte žiadosť o aplikáciu TeamViewer na zmeny v zariadení (len v systéme Windows).
7. Spustí sa aplikácia TeamViewer a obsahuje kód relácie na overenie pripojenia k vzdialenému zariadeniu.

**Časť 2: Na zariadení, ktoré je určené na vzdialenú reláciu**

1. Otvorte portál spoločnosti Intune.
2. Vyhľadajte príznak upozornenia: "Správca IT požaduje kontrolu nad týmto zariadením pre reláciu pomoci na diaľku a vyberte upozornenie.
3. Vyberte, či chcete stiahnuť aplikáciu TeamViewer, alebo potvrďte stiahnutie aplikácie TeamViewer z obchodu s aplikáciami a vyberte položku **Spustiť**.
    **Upozornenie:** Môžete ignorovať ľubovoľnú stránku webového prehľadávača otvorenú na webovej lokalite aplikácie TeamViewer.

4. Potvrďte žiadosť o aplikáciu TeamViewer na zmeny v zariadení (len v systéme Windows).
5. Spustí sa aplikácia TeamViewer a obsahuje kód relácie na overenie pripojenia k vzdialenému zariadeniu.
6. Kontextová ponuka sa zobrazí otázka, či chcete povoliť spustenie relácie.

**Upozornenie:** Kódy relácií generované službou TeamViewer sú len na jedno použitie. Ak stratíte pripojenie, musíte:

1. Zatvorte inštanciu aplikácie TeamViewer na vzdialenom zariadení a na pracovnej stanici správcu.
2. Zatvorte firemný portál na vzdialenom zariadení.
3. Inicializovať novú "Novú reláciu pomoci na diaľku" z portálu na správu.
4. Znova otvorte firemný portál na vzdialenom zariadení a dostanete nové upozornenie.
5. Stiahnite si a otvorte aplikáciu TeamViewer na vzdialenom zariadení aj na pracovnej stanici správcu, ako predtým.