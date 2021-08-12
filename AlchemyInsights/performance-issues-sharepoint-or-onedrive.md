---
title: Problémy s výkonom SharePoint alebo OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911857"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint alebo OneDrive pomalá, neprístupná alebo nedostupná pre viacerých používateľov

SharePoint služby OneDrive môžu byť pomalé, neprístupné alebo nedostupné, alebo môžu z viacerých dôvodov zobraziť nedostupnú službu alebo 503 chýb:
  
- Ak je vaša lokalita služieb SharePoint alebo OneDrive pomalá alebo oneskorená pre viacerých používateľov, môže ísť o dočasnú službu, pri ktorej sa používateľom pri prístupe k lokalitám SharePoint alebo OneDrive vyskytujú občasné oneskorenia alebo chyby OneDrive. Na [tabuli Stav služby](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) zistite, či to bude mať vplyv na vašu organizáciu.
  
- Používateľom sa môže zobraziť chyba *zaneprázdnenia servera 503* pri pokuse o prechod na iné SharePoint alebo OneDrive lokalít. Túto chybu môže spôsobovať obmedzovanie v rámci služby SharePoint siete. SharePoint Online používa obmedzovanie na udržiavanie optimálneho výkonu a spoľahlivosti služby SharePoint Online. Obmedzovanie zníži počet akcií používateľa alebo súbežných hovorov (podľa skriptu alebo kódu), aby sa zabránilo nadužívanie zdrojov. Ďalšie informácie o obmedzovanie nájdete v téme Ako sa vyhnúť obmedzeniam alebo [zablokovaniu v SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Ak sa pri klasickej **alebo** **modernej webovej** SharePoint alebo stránke vyskytuje pomalý výkon, stránky môžete analyzovať pomocou [nástroja](https://aka.ms/perftool) Diagnostika stránky.
  
- Ak stále máte všeobecný pomalý výkon, pozrite si zdroje v dolnej časti tohto článku: Úvod do ladenia výkonu [pre SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  