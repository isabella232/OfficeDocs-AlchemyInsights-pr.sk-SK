---
title: Problémy s vývojom aplikácií pomocou rozhrania API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975017"
---
# <a name="issues-developing-applications-with-apis"></a>Problémy s vývojom aplikácií pomocou rozhrania API

Ak chcete začať používať rozhranie API služby Azure Active Directory Graph, pozrite si príručku rozhrania API rýchlych reklám v službe [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) alebo zobrazenie [interaktívnej referenčnej dokumentácie rozhrania API služby Azure AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Koniec podpory pre Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph)**

**Od 30. júna 2020**, už nebudeme pridávať žiadne nové funkcie do služby ADAL a Azure AD Graph. Budeme aj naďalej poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudú poskytovať aktualizácie funkcií.

**Od 30. júna 2022**, ukončíme podporu pre ADAL a Azure AD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia.

Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však mať žiadne technické podpory ani aktualizácie zabezpečenia.

Aplikácie využívajúce Azure AD Graph po uplynutí tohto času už nemusia dostávať odpovede z koncového bodu služby Azure AD Graphu.

**Migrácia ADAL**

Odporúčame aktualizovať na [knižnicu Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ktorá obsahuje najnovšie funkcie a aktualizácie zabezpečenia.

Ak používate aplikácie spoločnosti Microsoft, viem, že spoločnosť Microsoft je v procese migrácie svojich aplikácií, aby MSAL podľa termínu ukončenia podpory, čím zabezpečí, že budú profitovať z priebežných vylepšení zabezpečenia a funkcií MSAL.

1. [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Zistite, ako migrovať aplikácie na základe jednotlivých platforiem](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Ak potrebujete pomoc s pochopením, ktoré z vašich aplikácií používajú ADAL, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a prípadne osloviť všetkých nezávislých poskytovateľov služieb alebo poskytovateľov aplikácií. Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií, ktoré nie sú Microsoft ADAL v nájomníkovi.

**Migrácia grafu AAD**

V prípade aplikácií, ktoré používajú Azure AD Graph, postupujte podľa pokynov na migráciu [aplikácií služby Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Náš kontrolný zoznam migrácie poskytuje bod začiatku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Na portáli registrácie aplikácie Azure sa zobrazuje, ktoré aplikácie používajú AAD Graph. Odporúčame, aby ste si prečítali všetky zdrojové kódy aplikácií a ak je to možné, Oslovte ľubovoľných poskytovateľov ISV alebo aplikácií. Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých použití AAD grafov v nájomníkovi.
1. Pre aplikáciu na prístup k údajom v programe Microsoft Graph musí používateľ alebo správca udeliť správne povolenia prostredníctvom procesu súhlasu. V [odkaze na povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) sú uvedené povolenia priradené k jednotlivým hlavným množinám rozhraní API programu Microsoft Graph. Poskytuje aj usmernenie o tom, ako používať povolenia.
