---
title: Prístup bol odmietnutý pri prezeraní pracovného postupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687345"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Prístup bol odmietnutý pri prezeraní pracovného postupu

SharePoint 2013 toky činností, ktoré sa pokúšajú odoslať e-mail skupiny SharePoint môže zlyhať s "prístup odmietnutý" chybové hlásenie, ak členstvo v skupine SharePoint nie je nastavená na všetky.
  
 **Ak chcete vyriešiť tento problém, postupujte nasledovne:**
  
 1. Umožním všetkým vidieť členov skupiny SharePoint.
  
 2. Odstráňte skupinu SharePoint z riadka Komu alebo kópia e-mailu.
  
 3. Explicitne pridať používateľov do riadka Komu alebo kópia, ak nie je možné zmeniť členstvo viditeľnosť pre skupinu SharePoint.
  
Ak chcete zobraziť ďalšie podrobnosti nájdete [http neoprávnené na/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  