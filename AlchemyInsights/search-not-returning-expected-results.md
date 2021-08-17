---
title: 1491-search-not-returning-expected-results
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
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052725"
---
# <a name="content-search-not-returning-expected-results"></a>Vyhľadávanie obsahu nevráti očakávané výsledky

Pri spustení vyhľadávania obsahu z Centra Microsoft 365 zabezpečenia & sa môžu zobraziť neočakávané výsledky hľadania. Vezmite do úvahy nasledujúce veci, ktoré môžu ovplyvniť výsledky hľadania:

- **Umiestnenia obsahu a podmienky vyhľadávania:** Skontrolujte, či ste vybrali správne umiestnenia obsahu a podmienky vyhľadávania. Ak ste spustili veľké vyhľadávanie (v mnohých umiestneniach), zvážte jeho rozdelenie na viacero vyhľadávaní.

- **Čiastočne indexované položky:**  [Čiastočne indexované položky z](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) poštových schránok sa zahrnú do odhadovaných výsledkov vyhľadávania. Čiastočne indexované položky z lokalít vo webových SharePoint a OneDrive nie sú zahrnuté v odhade vyhľadávania.

- Zlyhania **vyhľadávania:** Pri vyhľadávaní veľkého počtu poštových schránok (viac ako 100 000 poštových schránok) sa môžu zobraziť chyby vyhľadávania s kódmi chyby, ako sú napríklad CS008-009 a CS012-002). V takom prípade skúste znova vyhľadať iba neúspešné umiestnenia obsahu. Ďalšie  [informácie nájdete v](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) tomto článku.
