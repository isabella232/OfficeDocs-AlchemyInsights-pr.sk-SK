---
title: Dotazovanie rozhrania API programu Microsoft Graph
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974685"
---
# <a name="querying-the-microsoft-graph-api"></a>Dotazovanie rozhrania API programu Microsoft Graph

Táto téma sa môže vzťahovať aj na vývojárov, ktorí stále používajú rozhranie API služby Azure AD Graph. **Dôrazne** sa však odporúča používať program Microsoft Graph na všetky scenáre v adresári, identite a Accesse.

**Problémy s overovaním alebo autorizáciou**

- Ak vaša aplikácia **nedokáže získať tokeny** na volanie do programu Microsoft Graph, vyberte **problém s použitím kategórie accessových tokenov (Authentication)** pre Microsoft Graph a získajte konkrétnu pomoc a podporu v tejto téme.
- Ak vaša aplikácia **prijíma chyby autorizácie 401 alebo 403** pri volaní programu Microsoft Graph, vyberte položku **získať chybu odmietnutia prístupu (autorizácia)** Microsoft Graphu API, aby ste získali konkrétnu pomoc a podporu v tejto téme.

**Chcem použiť Microsoft Graph, ale nie ste si istí, kde začať**

Ďalšie informácie o programe Microsoft Graph nájdete v témach:

- [Prehľad programu Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Prehľad identity a riadenia prístupu v programe Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Začíname s budovaním aplikácií Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testovanie API programu Microsoft Graph v nájomníkovi alebo ukážkovom nájomníkovi

**Chcem používať Microsoft Graph, ale podporuje to rozhrania v 1.0 Directory API, ktoré potrebujem?**

Microsoft Graph je odporúčaný API pre adresár, identitu a riadenie prístupu. Existuje však niekoľko rozdielov medzi tým, čo je možné v službe Azure AD Graph a Microsoft Graph. Pozrite si nasledujúce články, ktoré zvýrazňujú najaktuálnejšie rozdiely na pomoc pri výbere:

- [Rozdiely v type zdroja medzi Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rozdiely medzi vlastnosťami medzi Azure AD Graphom a Microsoft Graphom](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Rozdiely v metóde medzi službou Azure AD a programom Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Pri dotaze na objekt *používateľa* chýbajú mnohé z jeho vlastností**

`GET https://graph.microsoft.com/v1.0/users` vráti iba 11 vlastností, pretože Microsoft Graph automaticky vyberie predvolenú množinu vlastností *používateľa* , ktorá sa má vrátiť. Ak potrebujete ďalšie vlastnosti *používateľa* , použite $Select na výber vlastností, ktoré potrebuje vaša aplikácia. Vyskúšajte si to v **programe Microsoft Graph Explorer** ako prvý.

**Niektoré hodnoty vlastností používateľa majú *hodnotu null* , aj keď viem, že sú nastavené**

Najpravdepodobnejšie vysvetlenie je, že žiadosť bola poskytnutá *používateľovi. ReadBasic. All* permission. To umožňuje aplikácii čítať obmedzenú množinu vlastností používateľa a vrátiť všetky ostatné vlastnosti ako hodnotu null aj v prípade, že boli predtým nastavené. Skúste udeliť používateľovi aplikácie *. read. All* povolenie namiesto toho.

Ďalšie informácie nájdete v téme [povolenia používateľov programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Mám problémy s používaním parametrov dotazu OData na filtrovanie údajov v mojich požiadavkách**

Zatiaľ čo Microsoft Graph podporuje širokú škálu parametrov OData dotazu, mnohé z týchto parametrov nie sú plne podporované v adresárových službách (zdroje, ktoré dedia z *directoryObject*) v Microsoft graphe. Rovnaké obmedzenia, ktoré boli prítomné v službe Azure AD Graphu, sú v Microsoft Graphe naďalej z veľkej časti:

1. **Nepodporované**: $count, $search a $filter s hodnotami *null* alebo *NOT NULL*
2. **Nie je podporované**: $filter na niektoré vlastnosti (pozrite tému zdroje informácií o tom, ktoré vlastnosti sú filtrované)
3. **Nepodporované**: stránkovanie, filtrovanie a zoraďovanie súčasne
4. **Nie je podporované**: filtrovanie vzťahu. Napríklad – vyhľadanie všetkých členov inžinierskej skupiny, ktoré sú vo Veľkej Británii.
5. **Čiastočná podpora**: $orderby na *používateľa* (iba DisplayName a userPrincipalName) a *skupina*
6. **Čiastočná podpora**: $filter (podporuje iba *EQ*, startswith *alebo*, *a* *a Limited)* podporu, $Expand (rozšírenie vzťahov jedného objektu vráti všetky vzťahy, ale rozšírenie skupiny vzťahov objektov je obmedzené) 

Ďalšie informácie nájdete v téme [Prispôsobenie odpovedí pomocou parametrov dotazu](https://docs.microsoft.com/graph/query-parameters).

**Volanie rozhrania API nefunguje – kde môžem vykonať ďalšie testovanie?**

**Microsoft Graph Explorer** – otestujte rozhrania API programu Microsoft Graph v nájomníkovi alebo ukážkovom nájomníkovi a pozrite si aj **vzorové dotazy** v programe Microsoft Graph Explorer.

**Pri dotaze na údaje sa zdá, že je naspäť neúplný súbor údajov**

Ak vytvárate dotaz na kolekciu (napríklad *Používatelia*), Microsoft Graph použije limity stránok na strane servera, takže výsledky sa vždy vrátia s predvolenou veľkosťou strany. Vaša aplikácia by mala vždy očakávať, že prejdete na stránku prostredníctvom kolekcií vrátených zo služby.

Ďalšie informácie nájdete v téme:

- [Najvhodnejšie postupy v programe Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Stránkovanie údajov programu Microsoft Graph v aplikácii](https://docs.microsoft.com/graph/paging)

**Moja aplikácia je príliš pomalá a je tiež stále obmedzovaná. Aké vylepšenia môžem urobiť?**

V závislosti od vášho scenára je k dispozícii široká škála rôznych možností, ktoré vám pomôžu vykonať viac výkonných aplikácií a v niektorých prípadoch menej náchylné na obmedzovanie službou (pri príliš veľkom počte hovorov).

Ďalšie informácie nájdete v témach:

- [Najvhodnejšie postupy v programe Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Požiadavky na dávkovanie](https://docs.microsoft.com/graph/json-batching)
- [Sledovanie zmien prostredníctvom Delta dotazu](https://docs.microsoft.com/graph/delta-query-overview)
- [Upozornenia na zmeny prostredníctvom webhookov](https://docs.microsoft.com/graph/webhooks)
- [Usmernenie o obmedzovaní](https://docs.microsoft.com/graph/throttling)

**Kde nájdem ďalšie informácie o chybách a známych problémoch?**

- [Informácie o odpovedaní na chyby v Microsoft Graphe](https://docs.microsoft.com/graph/errors)
- [Známe problémy s aplikáciou Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Kde môžem skontrolovať stav dostupnosti a pripojenia služby?**

Dostupnosť služieb a pripojenie k základným službám, ku ktorým je možné získať prístup prostredníctvom programu Microsoft Graph, môže mať vplyv na celkovú dostupnosť a výkon programu Microsoft Graph.

- Ak ide o stav služby Azure Active Directory, pozrite si stav služieb **zabezpečenia a identít** uvedených na [stránke stavu Azure](https://azure.microsoft.com/status/).
- V prípade služieb Office, ktoré prispievajú do programu Microsoft Graph, skontrolujte stav služieb uvedených v časti [Tabuľa stavu služieb balíka Office](https://portal.office.com/adminportal/home#/servicehealth).
