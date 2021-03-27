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
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398600"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Pokročilé koncepcie overovania platné pre Microsoft Edge

Nižšie sú uvedené pokročilé koncepty overovania, ktoré sa vzťahujú na Microsoft Edge:

**Proaktívne overovanie**

Po zapnutí politiky [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) sa Microsoft Edge pokúsi proaktívne overiť prihlásených používateľov prostredníctvom služieb spoločnosti Microsoft. V pravidelných intervaloch bude používať online službu na kontrolu aktualizovaného manifestu, ktorý obsahuje konfiguráciu, ktorá riadi proaktívne overovanie.

Výhody: Proaktívne overovanie umožňuje overovanie v kľúčových službách, ako je napríklad stránka Nová karta balíka Office. Ak sa ako vyhľadávací nástroj používa Bing, proaktívne overovanie zlepšuje výkon panela s adresou a pomáha generovať výsledky vyhľadávania prispôsobené potrebám vášho podniku.

**Overovanie Systému Windows Hello CredUI pre systém NTLM**

Ak jediné prihlásenie (SSO) nie je k dispozícii, keď sa webová lokalita pokúsi používateľa prihlásiť prostredníctvom mechanizmu NTLM alebo Vyjednať, táto funkcia umožní používateľovi zdieľať poverenia operačného systému s webovou lokalitu a splniť výzvu overenia pomocou používateľského rozhrania Windows Hello Cred. Tento tok prihlásenia sa zobrazí len vo Windowse 10 a len pre používateľov, ktorí nemajú jediné prihlásenie počas NTLM alebo vyjednania výzvu Vyjednať.

**Automatické prihlásenie pomocou uložených hesiel**

Používatelia, ktorí ukladajú heslá v Microsoft Edgei, môžu povoliť automatické prihlásenie na webové lokality, na ktorých uložili poverenia. Používatelia môžu túto funkciu v počítačovej edge://settings/passwords zapnúť alebo vypnúť a môžete ju nakonfigurovať v rámci politík [správcu hesiel.](https://go.microsoft.com/fwlink/?linkid=2134622)
