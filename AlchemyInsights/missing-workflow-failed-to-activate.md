---
title: Chýbajúci pracovný postup sa nepodarilo aktivovať
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762116"
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
  

