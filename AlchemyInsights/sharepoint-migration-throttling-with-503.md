---
title: SharePoint migrácie škrtenia s 503 chyby
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931673"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>SharePoint migrácie škrtenia s 503 chyby

**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí. Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania. Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.

Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa. Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch. Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.

**503 chyby pri migrácii SharePoint Online**

Zdá sa, že migrujete na SharePoint Online a prijímanie 503 chyby. Prosím, postupujte podľa nižšie uvedených krokov, aby sme vám mohli pomôcť čo najskôr. 

1. Kliknite na položku **kontaktovať technickú podporu**, a potom **novú servisnú požiadavku**.
2. Názov a popis, zadajte **SharePoint migrácie škrtenia s 503**.
3. Po tom, čo bol lístok predložený, aktualizujte ho s nasledujúcimi informáciami:
    - Koľko odišiel z migrácie (napríklad koľko TBs?).
    - Dátum začatia a ukončenia migrácie.
    - Opíšte, kam migrujete svoj obsah, napríklad SharePoint Server, box, GDrive, zdieľaných súborov atď.
    - Odhadnúť počet škrtenia chyby (napríklad x Throttle za hodinu?) a kedy sa škrtenia stalo.
    - Ktorý nástroj migrácie používate (napríklad SPMT alebo ShareGate).


