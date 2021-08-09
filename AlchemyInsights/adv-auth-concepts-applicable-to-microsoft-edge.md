---
title: Pokročilé koncepcie overovania platné pre Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934380"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Pokročilé koncepcie overovania platné pre Microsoft Edge

Nižšie sú uvedené pokročilé koncepty overovania, ktoré sa vzťahujú na Microsoft Edge:

**Proaktívne overovanie**

Keď povolíte politiku [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge sa pokúsi proaktívne overiť prihlásených používateľov prostredníctvom služby Microsoft. V pravidelných intervaloch bude používať online službu na kontrolu aktualizovaného manifestu, ktorý obsahuje konfiguráciu, ktorá riadi proaktívne overovanie.

Výhody: Proaktívne overenie umožňuje overovanie v kľúčových službách, ako je napríklad Office nová karta. Ak sa Bing ako vyhľadávací nástroj, proaktívne overovanie zlepšuje výkon panela s adresou a pomáha generovať výsledky hľadania prispôsobené potrebám vášho podniku.

**Windows Hello CredUI pre overovanie NTLM**

Ak jediné prihlásenie (SSO) nie je k dispozícii, keď sa webová lokalita pokúsi používateľa prihlásiť prostredníctvom mechanizmu NTLM alebo Vyjednať, táto funkcia umožní používateľovi zdieľať poverenia operačného systému s webovou lokalitu Windows Hello splniť výzvu overenia pomocou cred UI. Tento tok prihlásenia sa zobrazí len Windows 10 a len pre používateľov, ktorí nemajú jediné prihlásenie pri výzve NTLM alebo Vyjednať.

**Automatické prihlásenie pomocou uložených hesiel**

Používatelia, ktorí ukladajú heslá Microsoft Edge môžu povoliť automatické prihlásenie na webové lokality, na ktorých uložili poverenia. Používatelia môžu túto funkciu v počítačovej edge://settings/passwords zapnúť alebo vypnúť a môžete ju nakonfigurovať v rámci politík [správcu hesiel.](https://go.microsoft.com/fwlink/?linkid=2134622)
