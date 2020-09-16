---
title: 1491 – vyhľadávanie – nevracajú sa – očakávané – výsledky
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740489"
---
# <a name="content-search-not-returning-expected-results"></a>Vyhľadávanie obsahu nevracia očakávané výsledky

Pri spúšťaní vyhľadávania obsahu z centra zabezpečenia & zabezpečenia spoločnosti Microsoft 365 sa môžu zobraziť neočakávané výsledky vyhľadávania. Zvážte nasledujúce skutočnosti, ktoré môžu ovplyvniť výsledky vyhľadávania:

- **Umiestnenia obsahu a podmienky vyhľadávania**: Skontrolujte, či ste vybrali správne umiestnenia obsahu a podmienky vyhľadávania. Ak ste spustili veľké vyhľadávanie (s mnohými umiestneniami), zvážte rozdelenie na viacero vyhľadávaní.

- **Čiastočne indexované položky**:  [čiastočne indexované položky](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) z poštových schránok sú zahrnuté v odhadovaných výsledkoch hľadania. Čiastočne indexované položky z lokalít v SharePointe a OneDrive však nie sú zahrnuté v odhade vyhľadávania.

- **Zlyhanie vyhľadávania**: pri vyhľadávaní veľkého počtu poštových schránok (cez 100 000 poštových schránok) sa môžu zobraziť chyby vyhľadávania s kódmi chýb, ako sú napríklad CS008-009 a CS012-002). V tomto prípade zopakujte vyhľadávanie len v prípade zlyhaných umiestnení obsahu. Ďalšie informácie nájdete v  [tomto článku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
