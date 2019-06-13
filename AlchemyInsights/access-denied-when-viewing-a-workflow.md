---
title: Prístup odmietnutý pri zobrazení pracovného postupu
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883606"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Prístup odmietnutý pri zobrazení pracovného postupu

Pracovné postupy služby SharePoint 2013, ktoré sa pokúšajú odoslať e-mail do skupiny SharePoint môžu zlyhať s chybové hlásenie "Prístup odmietnutý" Ak členstvo skupiny lokality SharePoint nie je nastavený pre každého.
  
 **Ak chcete vyriešiť tento problém, postupujte nasledovne:**
  
 1. Aby všetci vidieť členom skupiny SharePoint.
  
 2. Odstráňte skupinu SharePoint z poľa Komu alebo Kópiazadajte riadok e-mailu.
  
 3. Výslovne pridať používateľov do poľa Komu alebo Kópiazadajte Ak členstvo viditeľnosť nemožno zmeniť skupinu lokality SharePoint.
  
Zobrazte viac podrobností nájdete [HTTP neoprávnené na /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  