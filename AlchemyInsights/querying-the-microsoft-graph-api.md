---
title: Dotazovanie rozhrania Microsoft Graph API
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
- "9004345"
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923254"
---
# <a name="querying-the-microsoft-graph-api"></a>Dotazovanie rozhrania Microsoft Graph API

Táto téma sa môže vzťahovať aj na vývojárov, ktorí ešte stále používajú Azure AD Graph API. Dôrazne sa však **odporúča používať** Microsoft Graph pre všetky scenáre správy adresárov, identity a prístupu.

**Problémy s overou alebo oprávnením**

- Ak vaša aplikácia nedokáže získať **tokeny** na volanie služby Microsoft Graph, vyberte možnosť Problém so získaním prístupového **tokenu (overovanie)** služby Microsoft Graph a získajte špecifickú pomoc a podporu pre túto tému.
- Ak sa vo vašej aplikácii pri volaní do služieb Microsoft Graph zobrazuje **chyba 401 alebo 403,** vyberte kategóriu Získanie chyby Pri odmietnutí prístupu **(Oprávnenie)** rozhrania API spoločnosti Microsoft Graph a získajte špecifickú pomoc a podporu na tejto téme.

**Chcem používať Microsoft Graph, ale neviem, kde začať**

Ďalšie informácie o aplikácii Microsoft Graph nájdete v téme:

- [Prehľad aplikácie Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Prehľad spravovania identity a prístupu v Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Začíname budovať aplikácie Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testovanie rozhraní GRAPH Microsoft API v nájomníkovi alebo v nájomníkovi demoverzácie

**Chcem používať službu Microsoft Graph, ale podporuje rozhrania API adresára v1.0, ktoré potrebujem?**

Microsoft Graph je odporúčané rozhranie API pre adresár, identitu a spravovanie prístupu. Medzi možnosťami služby Azure AD a služby Microsoft Graph však Graph. Pozrite si nasledujúce články, v ktorých sú zvýraznené najpopulárnejších rozdielov, ktoré vám môžu pomôcť pri výbere:

- [Rozdiely medzi typmi zdrojov v Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rozdiely vo vlastnosti medzi Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Rozdiely v metódach medzi Azure AD a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Pri dotaze *objektu* používateľa chýbajú mnohé jeho vlastnosti**

`GET https://graph.microsoft.com/v1.0/users`vráti iba 11 vlastností, pretože Graph automaticky vyberie predvolenú množinu *používateľských* vlastností, ktoré sa majú vrátiť. Ak potrebujete ďalšie *používateľské vlastnosti,* použite $select na výber vlastností, ktoré vaša aplikácia potrebuje. Vyskúšajte si to najprv **v prehliadači Microsoft Graph Explorer.**

**Niektoré hodnoty používateľských vlastností majú *hodnotu null* aj napriek tomu, že sú nastavené**

Najpravdepodobnejšie je, že aplikácii bolo udelené *povolenie User.ReadBasic.All.* Táto funkcia umožňuje aplikácii čítať obmedzenú množinu vlastností používateľa, ktorá vráti všetky ostatné vlastnosti ako null, a to aj v prípade, že boli predtým nastavené. Skúste radšej udeliť *aplikácii povolenie User.Read.All.*

Ďalšie informácie nájdete v téme [Povolenia používateľa Graph Microsoft.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Mám problémy s používaním parametrov dotazu OData na filtrovanie údajov v mojich žiadostiach**

Hoci microsoft Graph podporuje širokú škálu parametrov dotazu OData, mnohé z týchto parametrov nie sú plne podporované adresár službami (zdroje, ktoré dedia z *adresáraObject)* v službe Microsoft Graph. Rovnaké obmedzenia, ktoré sa nachádzali v službe Azure AD Graph naďalej vo väčšine prípadov v službe Microsoft Graph:

1. **Podporované:**$count, $search a $filter s *hodnotou null* *alebo nie s hodnotou* null
2. **Nie je podporované:**$filter niektorých vlastnostiach (pozrite si témy o zdrojoch, o ktorých sú vlastnosti filtrovateľné)
3. **Nie je** podporované: stránkovanie, filtrovanie a zoraďovanie v rovnakom čase
4. **Nie je** podporované: filtrovanie vzťahu. Môžete napríklad nájsť všetkých členov skupiny inžinierov v Spojenom kráľovstve.
5. **Čiastočná podpora:**$orderby *používateľa* (displayName a userPrincipalName) a *skupina*
6. **Čiastočná** podpora: $filter (podporuje iba *eq* *,* začína s , alebo *,* a *a* obmedzené všetky *)* podpory, $expand (rozšírenie vzťahov jedného objektu vráti všetky vzťahy, ale rozšírenie kolekcie vzťahov objektov je obmedzené)

Ďalšie informácie nájdete v téme [Prispôsobenie odpovedí pomocou parametrov dotazu.](https://docs.microsoft.com/graph/query-parameters)

**Volanie rozhrania API nefunguje – kde môžem robiť viac testovania?**

**Microsoft Graph Explorer** – Otestujte rozhrania API služby Microsoft Graph vo vašom nájomníkovi alebo v ukážkového nájomníka a pozrite si aj vzorové dotazy v Prehliadači Microsoft Graph Explorer. 

**Pri dotaze na údaje sa zdá, že sa mi znova nastavia neúplné údaje**

Ak dotazováte na kolekciu (napríklad *používateľov),* Microsoft Graph použije obmedzenia stránok na strane servera, aby sa výsledky vždy vrátili s predvolenou veľkosťou strany. Aplikácia by mala vždy očakávať, že sa budú stránkovať cez kolekcie vrátené zo služby.

Ďalšie informácie nájdete v téme:

- [Osvedčené postupy Graph Microsoftom](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging Microsoft Graph data in your app](https://docs.microsoft.com/graph/paging)

**Aplikácia je príliš pomalá a tiež je s obmedzeniami. Aké vylepšenia môžem vykonať?**

V závislosti od vášho scenára máte k dispozícii rôzne možnosti, ktoré sú k dispozícii, aby vaša aplikácia bola výkonnšia, a v niektorých prípadoch je menej pravdepodobné, že je na vás služba závislá (keď voláte priveľa).

Ďalšie informácie nájdete v témach:

- [Osvedčené postupy Graph Microsoftom](https://docs.microsoft.com/graph/best-practices-concept)
- [Žiadosti o dávku](https://docs.microsoft.com/graph/json-batching)
- [Sledovanie zmien prostredníctvom dotazu delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Oznámenia o zmenách prostredníctvom webových prehliadačov](https://docs.microsoft.com/graph/webhooks)
- [Pokyny na obmedzovanie](https://docs.microsoft.com/graph/throttling)

**Kde nájdem ďalšie informácie o chybách a známych problémoch?**

- [Informácie Graph odpovede na chybu v Microsofte](https://docs.microsoft.com/graph/errors)
- [Známe problémy so systémom Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Kde môžem skontrolovať stav dostupnosti služby a pripojiteľnosti?**

Dostupnosť služby a pripojenie základných služieb, ku ktoré je možné získať prístup prostredníctvom služby Microsoft Graph, môže ovplyvniť celkovú dostupnosť a výkon služieb spoločnosti Microsoft Graph.

- Ak Azure Active Directory služby, skontrolujte stav služieb **zabezpečenia a identity,** ktoré sú uvedené na [stránke so stavom služby Azure.](https://azure.microsoft.com/status/)
- Ak Office služby, ktoré prispievajú k službe Microsoft Graph, skontrolujte stav služieb uvedených na tabuli stavu služby [Office služby.](https://portal.office.com/adminportal/home#/servicehealth)
