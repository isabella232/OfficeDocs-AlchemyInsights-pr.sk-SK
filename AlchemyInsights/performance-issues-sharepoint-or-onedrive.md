---
title: Problémy s výkonom-SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068432"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint alebo OneDrive pomalé, nedostupné alebo nedostupné pre viacerých používateľov

SharePoint alebo OneDrive môže byť pomalé, nedostupné alebo nedostupné, alebo môže zobraziť službu nedostupné alebo 503 chyby, z niekoľkých dôvodov:
  
- Ak je lokalita SharePoint alebo OneDrive pomalá alebo oneskorená pre viacerých používateľov, môže existovať dočasný problém so službou, pri ktorom používatelia vyskytnú občasné oneskorenia alebo chyby navigácie pri prístupe k lokalitám SharePoint alebo k obsahu OneDrivu. Ak chcete zistiť, či je vaša organizácia ovplyvnená, skontrolujte [stav služby](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .
  
- Používatelia môžu získať *503 server je zaneprázdnený* chyba pri pokuse o navigáciu na lokality SharePoint alebo OneDrive. Táto chyba môže byť spôsobená škrtenia v službe SharePoint. SharePoint Online používa obmedzovanie zachovať optimálny výkon a spoľahlivosť služby SharePoint Online. Obmedzovanie obmedzuje počet používateľských akcií alebo súbežné volania (podľa skriptu alebo kódu), aby sa zabránilo nadvyužívaniu zdrojov. Ďalšie informácie o obmedzovanie vidieť, [vyhnúť sa škrtil alebo blokované SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ak sa stretnete s pomalým výkonom s **klasickou** alebo **modernou** lokalitou alebo stránkou lokality SharePoint, využite [diagnostický nástroj stránky](https://aka.ms/perftool) na analýzu strán.
  
- Ak stále skúsenosti všeobecné pomalý výkon, prečítajte si zdroje v spodnej časti tohto článku: [Úvod do ladenie výkonu pre SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  