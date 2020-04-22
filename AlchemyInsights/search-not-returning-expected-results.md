---
title: 1491-Search-not-vracajúci sa-očakávané-výsledky
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709242"
---
# <a name="content-search-not-returning-expected-results"></a>Vyhľadávanie obsahu nevracia očakávané výsledky

Pri spustení vyhľadávania obsahu z Microsoft 365 zabezpečenia & Compliance Center, môže sa zobraziť neočakávané výsledky vyhľadávania. Zvážte nasledujúce veci, ktoré môžu ovplyvniť výsledky vyhľadávania:

- **Umiestnenia obsahu a podmienky vyhľadávania**: Skontrolujte, či ste vybrali správne umiestnenia obsahu a podmienky vyhľadávania. Ak ste spustili veľké vyhľadávanie (s mnohými miestami), zvážte rozdelenie do viacerých vyhľadávaní.

- **Čiastočne indexované položky**: [čiastočne indexované položky](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) z poštových schránok sú zahrnuté v odhadovaných výsledkoch vyhľadávania. Čiastočne indexované položky z lokalít SharePoint a OneDrive však nie sú zahrnuté do odhadu vyhľadávania.

- **Zlyhanie vyhľadávania**: pri hľadaní veľkého počtu poštových schránok (viac ako 100 000 poštových schránok) sa môžu získať chyby vyhľadávania s kódmi chýb, ako sú napríklad CS008-009 a CS012-002). V tomto prípade zopakujte vyhľadávanie len pre neúspešné umiestnenia obsahu. Pozri [Tento článok](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) pre viac informácií.
