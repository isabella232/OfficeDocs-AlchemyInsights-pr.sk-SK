---
title: Prístup odmietnutý pri zobrazení pracovného postupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688817"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Prístup odmietnutý pri zobrazení pracovného postupu

Pracovné postupy SharePointu 2013, ktoré sa pokúšajú odoslať e-maily do skupiny SharePointu, môžu zlyhať s chybovým hlásením "prístup odmietnutý", ak členstvo v skupine SharePoint nie je nastavené na hodnotu všetci.
  
 **Ak chcete tento problém vyriešiť, vykonajte tieto kroky:**
  
 1. Povoliť každému Zobraziť členov skupiny SharePoint.
  
 2. Odstráňte skupinu SharePointu z riadku Komu alebo kópia e-mailu.
  
 3. Ak nie je možné zmeniť viditeľnosť členstva v skupine SharePoint, explicitne Pridajte používateľov do riadku Komu alebo kópia.
  
Ak chcete zobraziť ďalšie podrobnosti, prečítajte si [http neoprávnené na/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  