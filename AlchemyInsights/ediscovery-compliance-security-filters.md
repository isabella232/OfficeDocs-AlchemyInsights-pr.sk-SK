---
title: Počas vyhľadávania a exportu obsahu sa nevrátia žiadne výsledky
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101281"
---
# <a name="no-results-returned-during-content-searchexport"></a>Počas vyhľadávania a exportu obsahu sa nevrátia žiadne výsledky

Ak sa vyskytnú problémy s nasledujúcimi scenármi vyhľadávania eDiscovery:

- Funkcia vyhľadávania a exportu obsahu nevráti žiadne údaje ani neočakávané údaje
- Vyhľadávanie eDiscovery alebo export zlyhá

Môže to byť spôsobené určitými filtrami zabezpečenia súladu, ktoré nastavuje konkrétny správca a neboli komunikované všetkým správcom.

Ak chcete vyriešiť tento problém, skontrolujte, či môžu tieto problémy spôsobovať nejaké filtre zabezpečenia súladu:

1. Pripojenie prostredia Powershell centra zabezpečenia a dodržiavania súladu
2. Spustite nasledujúce commandlety:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Ďalšie informácie o filtroch zabezpečenia súladu nájdete v téme [Filtrovanie povolení pre vyhľadávanie obsahu.](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
