---
title: Problémy s overovaním knižníc
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063644"
---
# <a name="issues-with-authentication-libraries"></a>Problémy s overovaním knižníc

1. [Knižnice overovania platformy Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) sú uvedené v zoznamoch knižníc podporovaných spoločnosťou Microsoft a kompatibilných klientskych a middleware knižníc.
2. Knižnica Microsoft Authentication Library (MSAL) podporuje viacero [tokov overovania](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) , ktoré sa používajú v rôznych scenároch aplikácie.
3. Ak chcete overiť a získať tokeny, môžete v kóde inicializovať novú verejnú alebo dôvernú klientsku aplikáciu. Pri inicializácii klientskej aplikácie v knižnici Microsoft Authentication Library (MSAL) môžete nastaviť niekoľko možností konfigurácie. Ďalšie informácie nájdete v téme [možnosti konfigurácie aplikácie](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Koniec podpory pre Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph)**

**Od 30. júna 2020**, už nebudeme pridávať žiadne nové funkcie do služby ADAL a Azure AD Graph. Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.

**Od 30. júna 2022**, ukončíme podporu pre ADAL a Azure AD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia.

Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však *mať žiadne technické podpory ani aktualizácie zabezpečenia*.

Aplikácie využívajúce Azure AD Graph po uplynutí tohto času už nemusia dostávať odpovede z koncového bodu služby Azure AD Graphu.

**Migrácia ADAL**

Odporúčame aktualizovať na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) s najnovšími funkciami a aktualizáciami zabezpečenia.

Ak používate aplikácie spoločnosti Microsoft, viem, že spoločnosť Microsoft je v procese migrácie svojich aplikácií, aby MSAL podľa termínu ukončenia podpory, čím zabezpečí, že budú profitovať z pokračujúcich funkcií zabezpečenia a vylepšení MSAL.

Ďalšie informácie nájdete v téme:

1. [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informácie o migrácii aplikácií na platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ak potrebujete pomoc s pochopením, ktoré z vašich aplikácií používajú ADAL, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a prípadne osloviť všetkých nezávislých poskytovateľov služieb alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.

**Migrácia AAD Graph**

V prípade aplikácií, ktoré používajú Azure AD Graph, postupujte podľa pokynov na [migráciu aplikácií služby Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Náš kontrolný zoznam migrácie poskytuje bod začiatku.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Portál registrácie aplikácie Azure zobrazuje aplikácie, ktoré používajú AAD Graph. Odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a v prípade potreby kontaktovať poskytovateľov internetových služieb alebo poskytovateľov aplikácií. Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých použití AAD grafov v nájomníkovi.
3. Pre aplikáciu na prístup k údajom v programe Microsoft Graph musí používateľ alebo správca udeliť správne povolenia prostredníctvom procesu súhlasu. V [odkaze na povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) sú uvedené povolenia priradené k jednotlivým hlavným množinám rozhraní API programu Microsoft Graph. Poskytuje aj usmernenie o tom, ako používať povolenia.
