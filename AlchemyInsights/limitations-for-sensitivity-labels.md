---
title: Obmedzenia pre označenia citlivosti súborov Office v SharePoint a OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813166"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Obmedzenia pre označenia citlivosti súborov Office v SharePoint a OneDrive

Pri povolení označení citlivosti pre Office súborov v SharePoint a OneDrive uvedomte si požiadavky a obmedzenia, ktoré zahŕňajú:

- SharePoint Office OneDrive nemôžete spracovať niektoré súbory označené Office zašifrované z počítačových aplikácií, ak súbory obsahujú údaje PowerQuery, údaje uložené vlastnými doplnokmi alebo vlastné XML časti.
- SharePoint a OneDrive pre existujúce súbory, ktoré ste už zašifrovali pomocou označení Azure Information Protection (AIP), nepoužívajte označenia citlivosti automaticky. Použitie označení citlivosti na šifrované súbory: 
    - Uistite sa, že menovky AIP boli migrované a publikované v centre Microsoft 365 súladu.
    - Stiahnite si označené súbory a potom ich nahrajte do svojho pôvodného SharePoint alebo OneDrive umiestnenie.
- V prípade šifrovaných dokumentov nie je tlač podporovaná.

Ďalšie podrobnosti o obmedzeniach nájdete v téme Povolenie označení citlivosti pre [Office v SharePoint a OneDrive](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
