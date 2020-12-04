---
title: Rozšírené koncepty overovania platné pre Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573530"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Rozšírené koncepty overovania platné pre Microsoft Edge

Nižšie sú uvedené pokročilé overovacie koncepty, ktoré sa vzťahujú na Microsoft Edge:

**Proaktívne overovanie**

Keď povolíte politiku [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge sa bude pokúšať aktívne autentifikovať používateľov s prihlásením prostredníctvom služieb spoločnosti Microsoft. V pravidelných intervaloch bude používať online službu na vyhľadanie aktualizovaného manifestu, ktorý obsahuje konfiguráciu, ktorá sa riadi proaktívnym overovaním.

Výhody: proaktívne overovanie umožňuje overenie kľúčových služieb, ako je napríklad stránka na novej karte balíka Office. Aj v prípade, že sa Bing používa ako vyhľadávací nástroj, aktívne overovanie zlepšuje výkon panela s adresou a pomáha vytvárať výsledky vyhľadávania prispôsobené potrebám vášho podniku.

**Windows Hello CredUI pre overovanie NTLM**

Ak nie je k dispozícii jediné prihlásenie (SSO), keď sa webová lokalita pokúsi prihlásiť používateľa prostredníctvom protokolu NTLM alebo vyjednávacieho mechanizmu, táto funkcia umožní používateľovi zdieľať poverenia operačného systému s webovou lokalitou a splniť výzvu na overenie pomocou používateľského rozhrania Windows Hello Cred. Tento tok pri prihlasovaní sa zobrazí iba vo Windowse 10 a len pre používateľov, ktorí nezískajú SSO v priebehu protokolu NTLM alebo vyjednávacieho problému.

**Automatické prihlásenie pomocou uložených hesiel**

Používatelia, ktorí ukladajú heslá v prehliadači Microsoft Edge, môžu povoliť automatické prihlásenie na webové lokality, na ktorých boli uložené poverenia. Používatelia môžu túto funkciu zapnúť alebo vypnúť v edge://settings/passwords a môžete ju nakonfigurovať v politikách [správcu hesiel](https://go.microsoft.com/fwlink/?linkid=2134622) .
