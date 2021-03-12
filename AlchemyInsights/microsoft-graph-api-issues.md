---
title: Problémy s rozhraním Microsoft Graph API
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
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714520"
---
# <a name="microsoft-graph-api-issues"></a>Problémy s rozhraním Microsoft Graph API

Táto téma sa môže vzťahovať aj na vývojárov, ktorí stále používajú rozhranie API služby Azure AD Graph. **Dôrazne** sa však odporúča používať program Microsoft Graph na všetky scenáre v adresári, identite a Accesse.

**Problémy s overovaním alebo autorizáciou**

- Ak vaša aplikácia **nedokáže získať tokeny** na volanie do programu Microsoft Graph, vyberte **problém s použitím kategórie accessových tokenov (Authentication)** pre Microsoft Graph a získajte konkrétnu pomoc a podporu v tejto téme.
- Ak vaša aplikácia **prijíma chyby autorizácie 401 alebo 403** pri volaní programu Microsoft Graph, vyberte položku **získať chybu odmietnutia prístupu (autorizácia)** Microsoft Graphu API, aby ste získali konkrétnu pomoc a podporu v tejto téme.

**Chcem použiť Microsoft Graph, ale nie ste si istí, kde začať**

- [Prehľad programu Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Prehľad identity a riadenia prístupu v programe Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Začíname s budovaním aplikácií Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testovanie API programu Microsoft Graph v nájomníkovi alebo ukážkovom nájomníkovi

**Chcem používať Microsoft Graph, ale podporuje to rozhrania v 1.0 Directory API, ktoré potrebujem?**

Microsoft Graph je odporúčaný API pre adresár, identitu a riadenie prístupu. Existuje však niekoľko rozdielov medzi tým, čo je možné v službe Azure AD Graph a Microsoft Graph. Pozrite si nasledujúce články, ktoré zvýrazňujú najaktuálnejšie rozdiely na pomoc pri výbere:

- [Rozdiely v type zdroja medzi Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rozdiely medzi vlastnosťami medzi Azure AD Graphom a Microsoft Graphom](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Rozdiely v metóde medzi službou Azure AD a programom Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Volanie rozhrania API nefunguje – kde môžem vykonať ďalšie testovanie?**

**Microsoft Graph Explorer** – otestujte rozhrania API programu Microsoft Graph v nájomníkovi alebo ukážkovom nájomníkovi a pozrite si aj **vzorové dotazy** v programe Microsoft Graph Explorer.

**Moja aplikácia je príliš pomalá a je tiež stále obmedzovaná. Aké vylepšenia môžem urobiť?**

V závislosti od vášho scenára je k dispozícii široká škála možností, ktoré vám pomôžu vyrobiť svoju aplikáciu, a v niektorých prípadoch menej náchylné na obmedzovanie službou (pri vykonaní príliš veľkého počtu hovorov).

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

Chyby autorizácie v programe Microsoft Graph môžu byť výsledkom niekoľkých rôznych problémov, z ktorých väčšina vygeneruje chybu 401 alebo 403. Tieto chyby môžu viesť napríklad k chybám autorizácie:

- Nesprávne [toky akvizície prístupového tokenu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Zle nakonfigurované [rozsahy povolení](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Chýbajúci [súhlas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Ukončenie podpory pre križnicu Azure Active Directory Authentication Library (ADAL) a rozhranie Azure AD Graph API (AAD Graph)_* _

_ * Od 30. júna 2020 * * už nebudeme pridávať žiadne nové funkcie do služby ADAL a Azure AD Graph. Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.

**Od 30. júna 2022**, ukončíme podporu pre ADAL a Azure AD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia.

Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však *mať žiadne technické podpory ani aktualizácie zabezpečenia*.

Aplikácie využívajúce Azure AD Graph po uplynutí tohto času už nemusia dostávať odpovede z koncového bodu služby Azure AD Graphu.

**Migrácia ADAL**

Odporúčame aktualizovať na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) s najnovšími funkciami a aktualizáciami zabezpečenia.

Ak používate aplikácie spoločnosti Microsoft, viem, že spoločnosť Microsoft je v procese migrácie svojich aplikácií, aby MSAL podľa termínu ukončenia podpory, čím zabezpečí, že budú profitovať z priebežných vylepšení zabezpečenia a funkcií MSAL.

1. [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informácie o migrácii aplikácií na platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ak potrebujete pomoc s pochopením, ktoré z vašich aplikácií používajú ADAL, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a prípadne osloviť všetkých nezávislých poskytovateľov služieb alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.

**Migrácia AAD Graph**

V prípade aplikácií, ktoré používajú Azure AD Graph, postupujte podľa pokynov na [migráciu aplikácií služby Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Náš kontrolný zoznam migrácie obsahuje informácie na začiatok](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Portál registrácie aplikácie Azure zobrazuje aplikácie, ktoré používajú AAD Graph. Odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a v prípade potreby kontaktovať poskytovateľov internetových služieb alebo poskytovateľov aplikácií. Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých použití AAD grafov v nájomníkovi.
3. Pre aplikáciu na prístup k údajom v programe Microsoft Graph musí používateľ alebo správca udeliť správne povolenia prostredníctvom procesu súhlasu. V [odkaze na povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) sú uvedené povolenia priradené k jednotlivým hlavným množinám rozhraní API programu Microsoft Graph. Poskytuje aj usmernenie o tom, ako používať povolenia.
