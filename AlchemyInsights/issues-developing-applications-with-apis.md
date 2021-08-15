---
title: Problémy pri vývoji aplikácií s rozhraniami API
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013475"
---
# <a name="issues-developing-applications-with-apis"></a>Problémy pri vývoji aplikácií s rozhraniami API

Ak chcete začať používať rozhranie Azure Active Directory Graph API, pozrite si príručku so [stručným návodom](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) k rozhraniu Azure AD Graph API alebo si pozrite interaktívnu referenčnú dokumentáciu [k rozhraniu AZURE AD Graph API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Ukončenie podpory pre Azure Active Directory overovanie (ADAL) a Azure AD Graph API (AAD Graph)**

**Od 30. júna 2020** už nebudeme do služieb ADAL a Azure AD Graph. Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.

**Od 30. júna 2022** ukončíme podporu pre ADAL a Azure AD Graph a už nebudeme poskytovať technickú podporu ani aktualizácie zabezpečenia.

Aplikácie používajúce ADAL v existujúcich verziách operačného systému budú fungovať aj naďalej, ale nebudú mať k dispozícii žiadnu technickú podporu ani aktualizácie zabezpečenia.

Aplikácie používajúce Azure AD Graph po tomto čase už nemusia dostávať odpovede z koncového bodu služby Azure AD Graph Ad.

**Migrácia ADAL**

Odporúčame aktualizovať na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) s najnovšími funkciami a aktualizáciami zabezpečenia.

Ak používate aplikácie spoločnosti Microsoft, znamená to, že spoločnosť Microsoft do termínu ukončenia podpory migruje aplikácie do služby MSAL, čím sa zabezpečí, že budú môcť využívať vylepšenia priebežného zabezpečenia a funkcií spoločnosti MSAL.

1. [Prečítajte si najčastejšie otázky o službe ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Získajte informácie o migrácii aplikácií na báze platformy.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Ak potrebujete pomoc s tým, ktoré aplikácie používajú ADAL, odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a ak je to možné, kontaktovať niektoré súbory ISVs alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.

**Migrácia AAD Graph**

V prípade aplikácií, ktoré používajú Azure AD Graph, postupujte podľa našich pokynov na migráciu aplikácií [Azure AD Graph do služby Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Náš kontrolný zoznam migrácie obsahuje informácie na začiatok](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Portál registrácie aplikácie Azure zobrazuje aplikácie, ktoré používajú AAD Graph. Odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a v prípade potreby kontaktovať poskytovateľov internetových služieb alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých použití služby AAD Graph v nájomníkovi.
1. Na prístup k údajom v aplikácii Microsoft Graph musí používateľ alebo správca udeliť správne povolenia prostredníctvom procesu súhlasu. Odkaz [na povolenia Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) Obsahuje zoznam povolení priradených ku každej hlavnej množine rozhraní API Microsoft Graph Microsoft. Poskytuje tiež pokyny na používanie povolení.
