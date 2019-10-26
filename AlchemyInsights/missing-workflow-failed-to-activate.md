---
title: Chýbajúci pracovný postup sa nepodarilo aktivovať
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36753811"
---
# <a name="missing-workflow-failed-to-activate"></a>Chýbajúci pracovný postup sa nepodarilo aktivovať

V kolekcii lokality Microsoft SharePoint, nemôžete pridať globálne opakovane pracovného postupu (napríklad "schválenie-SharePoint 2010") do zoznamu alebo knižnice.
  
Ak chcete vyriešiť tento problém, postupujte nasledovne: 
  
1. Otvorte koreňovú webovú lokalitu kolekcie lokalít v programe SharePoint Designer 2013.
  
2. V časti **objekty lokality**vyberte položku **toky činností**. 
  
3. V **novej** časti pása s nástrojmi **pracovné postupy** , vyberte **opakovane použiteľný pracovný postup**. 
  
4. Vo formulári **vytvoriť opakovane použiteľný pracovný postup** zadajte názov * * *Repair2010* * *. Pre **platformu typ**, kliknite na tlačidlo **SharePoint 2010 workflow**, a potom kliknite na **tlačidlo OK**. 
  
1. V časti **Uložiť** na páse s nástrojmi **pracovného postupu** vyberte **Publikovať**. 
  
2. V časti **Správa** pása s nástrojmi **pracovného postupu** vyberte položku **Publikovať globálne**. V zobrazenom dialógovom okne s potvrdením vyberte položku **OK**. 
  
3. Vo webovom prehľadávači vyhľadajte koreňovú webovú lokalitu kolekcie lokalít a **potom prístup k** \> **funkciám kolekcie**lokality. Potom prepnite funkciu **toky činností** : 
  
· Ak je funkcia *aktivovaná* , kliknite na tlačidlo **deaktivovať** a potom kliknite na tlačidlo **aktivovať**. 
  
· Ak je funkcia *deaktivovaná* , kliknite na tlačidlo **aktivovať**. 
  
Ďalšie informácie nájdete v nasledujúcom [článku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

