---
title: Prístup bol odmietnutý pri prezeraní pracovného postupu
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747763"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Prístup bol odmietnutý pri prezeraní pracovného postupu

SharePoint 2013 toky činností, ktoré sa pokúšajú odoslať e-mail skupiny SharePoint môže zlyhať s "prístup odmietnutý" chybové hlásenie, ak členstvo v skupine SharePoint nie je nastavená na všetky.
  
 **Ak chcete vyriešiť tento problém, postupujte nasledovne:**
  
 1. Umožním všetkým vidieť členov skupiny SharePoint.
  
 2. Odstráňte skupinu SharePoint z riadka Komu alebo kópia e-mailu.
  
 3. Explicitne pridať používateľov do riadka Komu alebo kópia, ak nie je možné zmeniť členstvo viditeľnosť pre skupinu SharePoint.
  
Ak chcete zobraziť ďalšie podrobnosti nájdete [http neoprávnené/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  