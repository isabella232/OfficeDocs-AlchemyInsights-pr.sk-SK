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
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955216"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Prístup odmietnutý pri zobrazení pracovného postupu

Pracovné postupy balíka SharePoint 2013, ktoré sa pokúšajú odoslať e-mail skupine vo SharePoint, môžu zlyhať s chybým "Prístup odmietnutý", ak členstvo v skupine SharePoint nie je nastavené na možnosť Všetci.
  
 **Ak chcete tento problém vyriešiť, postupujte takto:**
  
 1. Umožniť všetkým zobraziť členov tejto SharePoint skupiny.
  
 2. Odstráňte SharePoint e-mailu z riadka Komu alebo Kópia.
  
 3. Explicitne pridajte používateľov do riadka Komu alebo Kópia, ak sa viditeľnosť členstva nedá zmeniť SharePoint skupiny.
  
Ak chcete zobraziť ďalšie podrobnosti, pozrite si časť HTTP Neoprávnené do [/_vti_bin/client.svc/sp.utilities.utility.SendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  