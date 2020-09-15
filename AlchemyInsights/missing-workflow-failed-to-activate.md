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
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667101"
---
# <a name="missing-workflow-failed-to-activate"></a>Chýbajúci pracovný postup sa nepodarilo aktivovať

V kolekcii lokalít Microsoft SharePoint nie je možné do zoznamu alebo knižnice pridať globálne opätovne použiteľný pracovný postup (ako je napríklad "schválenie – SharePoint 2010").
  
Ak chcete tento problém vyriešiť, postupujte podľa týchto krokov: 
  
1. Otvorte koreňovú webovú lokalitu kolekcie lokalít v SharePointe Designeri 2013.
  
2. V časti **objekty lokality**vyberte položku **pracovné postupy**. 
  
3. V **novej** časti pása s nástrojmi **pracovných postupov** vyberte položku **opätovne použiteľný pracovný postup**. 
  
4. Na formulári **vytvoriť opätovne použiteľný pracovný postup** zadajte názov * * *Repair2010* * *. Pre **typ platformy**kliknite na položku **pracovný postup SharePointu 2010**a potom kliknite na tlačidlo **OK**. 
  
1. V časti **Uložiť** na páse s nástrojmi **pracovný postup** vyberte položku **Publikovať**. 
  
2. V časti **Spravovať** na páse s nástrojmi **pracovný postup** vyberte položku **Publikovať na globálnej úrovni**. V zobrazenom dialógovom okne potvrdenia vyberte položku **OK**. 
  
3. Vo webovom prehliadači vyhľadajte koreňovú webovú lokalitu kolekcie lokalít a potom kliknite na položku funkcie kolekcie lokalít v **časti Nastavenie lokality** \> **Site Collection Features**. Potom prepnite funkciu **pracovné postupy** : 
  
· Ak je funkcia  *aktivovaná*  , kliknite na položku **deaktivovať** a potom kliknite na položku **aktivovať**. 
  
· Ak je funkcia  *deaktivovaná*  , kliknite na položku **aktivovať**. 
  
Ďalšie informácie nájdete v nasledujúcom [článku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

