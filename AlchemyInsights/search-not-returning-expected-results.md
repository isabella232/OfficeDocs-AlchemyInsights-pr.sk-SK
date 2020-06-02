---
title: 1491-vyhľadávanie-ne-návrat-očakávané výsledky
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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510587"
---
# <a name="content-search-not-returning-expected-results"></a>Vyhľadávanie obsahu nevracia očakávané výsledky

Pri spustení vyhľadávania obsahu z Microsoft 365 zabezpečenia & Compliance Center, môže sa zobraziť neočakávané výsledky vyhľadávania. Zvážte nasledujúce možnosti, ktoré môžu ovplyvniť výsledky vyhľadávania:

- **Umiestnenia obsahu a podmienky vyhľadávania**: Uistite sa, že ste vybrali správne umiestnenia obsahu a podmienky vyhľadávania. Ak ste spustili veľké vyhľadávanie (s mnohými umiestneniami), zvážte jeho rozdelenie na viacero vyhľadávaní.

- **Čiastočne indexované položky**: [Čiastočne indexované položky](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) z poštových schránok sú zahrnuté vo výsledkoch odhadovaného vyhľadávania. Čiastočne indexované položky z lokalít SharePointu a OneDrivu však nie sú zahrnuté do odhadu vyhľadávania.

- **Zlyhania vyhľadávania**: Pri vyhľadávaní veľkého počtu poštových schránok (viac ako 100 000 poštových schránok) sa môžu zobraziť chyby vyhľadávania s chybovými kódmi, ako sú CS008-009 a CS012-002). V takom prípade zopakujte vyhľadávanie len pre neúspešné umiestnenia obsahu. Ďalšie informácie nájdete v [tomto článku.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)
