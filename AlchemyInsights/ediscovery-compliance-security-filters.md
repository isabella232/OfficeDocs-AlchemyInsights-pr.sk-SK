---
title: Pri vyhľadávaní obsahu alebo exportovaní sa nevrátia žiadne výsledky
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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680327"
---
# <a name="no-results-returned-during-content-searchexport"></a>Pri vyhľadávaní obsahu alebo exportovaní sa nevrátia žiadne výsledky

Ak sa vyskytnú problémy s nasledujúcimi scenármi eDiscovery:

- Vyhľadávanie obsahu/export vráti žiadne údaje ani neočakávané údaje
- Vyhľadávanie eDiscovery alebo export zlyhá

Môže to byť spôsobené určitými filtrami zabezpečenia súladu, ktoré boli nastavené konkrétnym správcom, a neboli oznámené všetkým správcom.

Ak chcete tento problém vyriešiť, skontrolujte, či sú k dispozícii žiadne filtre zabezpečenia súladu, ktoré môžu spôsobovať tieto problémy:

1. Pripojenie k centru PowerShell zabezpečenia a dodržiavania súladu
2. Spustite nasledovné príkazové aplety:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Ďalšie informácie o filtroch zabezpečenia dodržiavania súladu nájdete v téme [filtrovanie povolení na vyhľadávanie obsahu](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
