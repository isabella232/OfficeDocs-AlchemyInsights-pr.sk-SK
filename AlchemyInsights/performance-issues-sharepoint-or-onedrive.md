---
title: Problémy s výkonom – SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771916"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>Služby SharePoint alebo OneDrive sú pomalé, nedostupné alebo nie sú k dispozícii pre viacerých používateľov

SharePoint alebo OneDrive môže byť pomalý, nedostupný alebo nedostupný alebo môže zobraziť služby nedostupné alebo 503 chyby z niekoľkých dôvodov:
  
- Ak je lokalita SharePoint alebo OneDrive v prípade viacerých používateľov pomalá alebo oneskorená, môže sa vyskytnúť dočasný problém so službou, v ktorom používatelia vyskytnú občasné oneskorenia alebo chyby navigácie pri prístupe k lokalitám SharePoint alebo k obsahu OneDrivu. Ak chcete zistiť, či je vaša organizácia ovplyvnená, pozrite si [tabuľu stavu služby](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .
  
- Pri pokuse o prechod na lokalitu SharePoint alebo OneDrive môžu používatelia získať *server 503 je zaneprázdnená* chyba. Táto chyba môže byť spôsobená obmedzovaním v rámci služby SharePoint. SharePoint Online používa obmedzovanie na udržiavanie optimálneho výkonu a spoľahlivosti služby SharePoint Online. Obmedzovanie zníži počet akcií používateľa alebo súbežných hovorov (podľa skriptu alebo kódu), aby sa zabránilo nadužívanie zdrojov. Ďalšie informácie o obmedzovaní nájdete v téme [zamedzenie obmedzovania alebo blokovania v SharePointe Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ak sa stretnete s pomalým výkonom s **klasickou** alebo **modernou** lokalitou alebo stránkou SharePointu, využite [nástroj na diagnostiku stránky](https://aka.ms/perftool) na analýzu stránok.
  
- Ak sa stále vyskytuje všeobecný pomalý výkon, pozrite si zdroje v spodnej časti tohto článku: [úvodné informácie o ladení výkonu pre SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  