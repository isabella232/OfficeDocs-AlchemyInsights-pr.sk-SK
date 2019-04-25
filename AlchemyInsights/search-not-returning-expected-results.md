---
title: 1491-Search-not-Returning-Expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383850"
---
# <a name="content-search-not-returning-expected-results"></a>Obsah vyhľadávanie nevracajú očakávané výsledky

Pri spustení obsah vyhľadávanie od & Office 365 zabezpečenia súladu Center, dostanete neočakávané výsledky. Zoberme si nasledujúce veci, ktoré môžu ovplyvniť výsledky vyhľadávania:

- **Umiestnenia obsahu a podmienok vyhľadávania**: Uistite sa, že ste si vybrali správneho umiestnenia obsahu a vyhľadávanie podmienky. Ak ste spustili veľké vyhľadávanie (s mnohých miestach), zvážte ju rozdeliť na niekoľko prehliadok.

- **Čiastočne indexované položky**: [čiastočne indexované položky](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) zo schránky sú zahrnuté vo výsledkoch vyhľadávania odhadované. Však čiastočne indexované položky z lokalít v službe SharePoint a OneDrive nie sú zahrnuté v odhade Hľadať.

- **Vyhľadávanie porúch**: pri hľadaní veľkého počtu poštových schránok (viac ako 100.000 schránky), dostanete Hľadať chyby, kódy chýb ako je CS008-009 a CS012-002). V takom prípade zopakujte hľadanie zlyhalo obsah umiestnenia. Pozri [Tento článok](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pre viac informácií.
