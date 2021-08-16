---
title: Chýbajúci pracovný postup sa nepodarilo aktivovať
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065443"
---
# <a name="missing-workflow-failed-to-activate"></a>Chýbajúci pracovný postup sa nepodarilo aktivovať

V kolekcii lokalít služby Microsoft SharePoint nie je možné do zoznamu alebo knižnice pridať globálne opätovne použiteľný pracovný postup (napríklad Schválenie – SharePoint 2010).
  
Ak chcete tento problém vyriešiť, postupujte takto: 
  
1. V programe SharePoint Designer 2013 otvorte koreňovú webovú lokalitu kolekcie lokalít.
  
2. V **časti Objekty lokality** vyberte položku Pracovné **postupy**. 
  
3. V časti **Nové** na páse s **nástrojmi Pracovné postupy** vyberte položku Opätovne použiteľný pracovný **postup.** 
  
4. Vo formulári **Vytvoriť opätovne použiteľný pracovný** postup zadajte názov ** *Opraviť2010* **. V **prípade typu platformy** kliknite **na položku SharePoint 2010 Workflow** a potom kliknite na tlačidlo **OK.** 
  
1. V časti **Uložiť na** páse s **nástrojmi pracovného** postupu vyberte položku **Publikovať**. 
  
2. V časti **Spravovať na** páse s **nástrojmi pracovného** postupu vyberte položku **Publikovať globálne.** V zobrazenom potvrdzovacom dialógovom okne vyberte tlačidlo **OK.** 
  
3. Vo webovom prehliadači vyhľadajte koreňovú webovú lokalitu kolekcie lokalít a potom prejdite na **položku** Nastavenia \> **funkcie kolekcie lokalít.** Potom prepnite **funkciu pracovných** postupov: 
  
· Ak je funkcia  *aktivovaná, kliknite na*  položku **Deaktivovať a** potom na položku **Aktivovať**. 
  
· Ak je funkcia  *Deaktivovaná, kliknite*  na položku **Aktivovať**. 
  
Ďalšie informácie nájdete v nasledujúcom [článku.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

