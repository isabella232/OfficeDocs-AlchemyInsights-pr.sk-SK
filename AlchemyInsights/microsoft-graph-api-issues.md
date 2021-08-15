---
title: Problémy s rozhraním API Graph Microsoft Graph
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
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975908"
---
# <a name="microsoft-graph-api-issues"></a>Problémy s rozhraním API Graph Microsoft Graph

Táto téma sa môže vzťahovať aj na vývojárov, ktorí ešte stále používajú Azure AD Graph API. Dôrazne sa však **odporúča používať** Microsoft Graph pre všetky scenáre správy adresárov, identity a prístupu.

**Problémy s overou alebo oprávnením**

- Ak vaša aplikácia nedokáže získať **tokeny** na volanie služby Microsoft Graph, vyberte možnosť Problém so získaním prístupového **tokenu (overovanie)** služby Microsoft Graph a získajte špecifickú pomoc a podporu pre túto tému.
- Ak sa vo vašej aplikácii pri volaní do služieb Microsoft Graph zobrazuje **chyba 401 alebo 403,** vyberte kategóriu Získanie chyby Pri odmietnutí prístupu **(Oprávnenie)** rozhrania API spoločnosti Microsoft Graph a získajte špecifickú pomoc a podporu na tejto téme.

**Chcem používať Microsoft Graph, ale neviem, kde začať**

- [Prehľad aplikácie Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Prehľad spravovania identity a prístupu v Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Začíname budovať aplikácie Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testovanie rozhraní GRAPH Microsoft API v nájomníkovi alebo v nájomníkovi demoverzácie

**Chcem používať službu Microsoft Graph, ale podporuje rozhrania API adresára v1.0, ktoré potrebujem?**

Microsoft Graph je odporúčané rozhranie API pre adresár, identitu a spravovanie prístupu. Medzi možnosťami služby Azure AD a služby Microsoft Graph však Graph. Pozrite si nasledujúce články, v ktorých sú zvýraznené najpopulárnejších rozdielov, ktoré vám môžu pomôcť pri výbere:

- [Rozdiely medzi typmi zdrojov v Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rozdiely vo vlastnosti medzi Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Rozdiely v metódach medzi Azure AD a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Volanie rozhrania API nefunguje – kde môžem testovať viac?**

**Microsoft Graph Explorer** – Otestujte rozhrania API služby Microsoft Graph vo vašom nájomníkovi alebo v ukážkového nájomníka a pozrite si aj vzorové dotazy v Prehliadači Microsoft Graph Explorer. 

**Aplikácia je príliš pomalá a tiež je s obmedzeniami. Aké vylepšenia môžem vykonať?**

V závislosti od vášho scenára máte k dispozícii rôzne možnosti, ktoré sú k dispozícii, aby vaša aplikácia bola výkonnšia, a v niektorých prípadoch je menej pravdepodobné, že je na vás služba závislá (keď voláte priveľa).

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

Chyby Graph v oprávneniach od spoločnosti Microsoft môžu byť výsledkom niekoľkých rôznych problémov, z ktorých väčšina generuje chybu 401 alebo 403. Chyby v oprávneniach môžu viesť napríklad k týmto chybám:

- Nesprávne [toky akvizície prístupového tokenu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Zle nakonfigurované [rozsahy povolení](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Chýbajúci [súhlas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Ukončenie podpory pre Azure Active Directory overovanie (ADAL) a Azure AD Graph API (AAD Graph)***

**Od 30. júna 2020** už nebudeme do služieb ADAL a Azure AD Graph. Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.

**Od 30. júna 2022** ukončíme podporu pre ADAL a Azure AD Graph a už nebudeme poskytovať technickú podporu ani aktualizácie zabezpečenia.

Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú po tomto čase naďalej fungovať, nebudú však môcť získať *žiadnu technickú podporu ani aktualizácie zabezpečenia.*

Aplikácie používajúce Azure AD Graph po tomto čase už nemusia dostávať odpovede z koncového bodu služby Azure AD Graph Ad.

**Migrácia ADAL**

Odporúčame aktualizovať na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) s najnovšími funkciami a aktualizáciami zabezpečenia.

Ak používate aplikácie spoločnosti Microsoft, znamená to, že spoločnosť Microsoft do termínu ukončenia podpory migruje aplikácie do služby MSAL, čím sa zabezpečí, že budú môcť využívať vylepšenia priebežného zabezpečenia a funkcií spoločnosti MSAL.

1. [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informácie o migrácii aplikácií na platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ak potrebujete pomoc s tým, ktoré aplikácie používajú ADAL, odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a ak je to možné, kontaktovať niektoré súbory ISVs alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.

**Migrácia AAD Graph**

V prípade aplikácií, ktoré používajú Azure AD Graph, postupujte podľa našich pokynov na migráciu aplikácií [Azure AD Graph do služby Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Náš kontrolný zoznam migrácie obsahuje informácie na začiatok](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Portál registrácie aplikácie Azure zobrazuje aplikácie, ktoré používajú AAD Graph. Odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a v prípade potreby kontaktovať poskytovateľov internetových služieb alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých použití služby AAD Graph v nájomníkovi.
3. Na prístup k údajom v aplikácii Microsoft Graph musí používateľ alebo správca udeliť správne povolenia prostredníctvom procesu súhlasu. Odkaz [na povolenia Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference) Obsahuje zoznam povolení priradených ku každej hlavnej množine rozhraní API Microsoft Graph Microsoft. Poskytuje tiež pokyny na používanie povolení.
