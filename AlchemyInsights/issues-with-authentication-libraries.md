---
title: Problémy s knižnicami overovania
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
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028019"
---
# <a name="issues-with-authentication-libraries"></a>Problémy s knižnicami overovania

1. [Microsoft identity platform overovanie zoznamov knižníc](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) klienta a middleware podporovaných spoločnosťou Microsoft.
2. Knižnica Microsoft Authentication Library (MSAL) podporuje [niekoľko](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) tokov overenia na použitie v rôznych scenároch aplikácií.
3. Ak chcete overiť a získať tokeny, inicializujete novú verejnú alebo dôvernú klientsku aplikáciu v kóde. Pri inicializácii klientskej aplikácie v knižnici overovania spoločnosti Microsoft (MSAL) môžete nastaviť niekoľko možností konfigurácie. Ďalšie informácie nájdete v téme [Možnosti konfigurácie aplikácie.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Ukončenie podpory pre Azure Active Directory overovanie (ADAL) a Azure AD Graph API (AAD Graph)**

**Od 30. júna 2020** už nebudeme do služieb ADAL a Azure AD Graph. Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.

**Od 30. júna 2022** ukončíme podporu pre ADAL a Azure AD Graph a už nebudeme poskytovať technickú podporu ani aktualizácie zabezpečenia.

Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú po tomto čase naďalej fungovať, nebudú však môcť získať *žiadnu technickú podporu ani aktualizácie zabezpečenia.*

Aplikácie používajúce Azure AD Graph po tomto čase už nemusia dostávať odpovede z koncového bodu služby Azure AD Graph Ad.

**Migrácia ADAL**

Odporúčame aktualizovať na [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) s najnovšími funkciami a aktualizáciami zabezpečenia.

Ak používate aplikácie spoločnosti Microsoft, znamená to, že spoločnosť Microsoft do termínu ukončenia podpory migruje aplikácie do služby MSAL, čím sa zabezpečí, že budú môcť využívať vylepšenia priebežného zabezpečenia a funkcií spoločnosti MSAL.

Ďalšie informácie nájdete v téme:

1. [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informácie o migrácii aplikácií na platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ak potrebujete pomoc s tým, ktoré aplikácie používajú ADAL, odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a ak je to možné, kontaktovať niektoré súbory ISVs alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.

**Migrácia AAD Graph**

V prípade aplikácií, ktoré používajú Azure AD Graph, postupujte podľa našich pokynov na migráciu aplikácií [Azure AD Graph do služby Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Náš kontrolný zoznam migrácie poskytuje priestor na začiatok.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Portál registrácie aplikácie Azure zobrazuje aplikácie, ktoré používajú AAD Graph. Odporúčame vám skontrolovať zdrojový kód všetkých aplikácií a v prípade potreby kontaktovať poskytovateľov internetových služieb alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých použití služby AAD Graph v nájomníkovi.
3. Na prístup k údajom v aplikácii Microsoft Graph musí používateľ alebo správca udeliť správne povolenia prostredníctvom procesu súhlasu. Odkaz [na povolenia Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference) Obsahuje zoznam povolení priradených ku každej hlavnej množine rozhraní API Microsoft Graph Microsoft. Poskytuje tiež pokyny na používanie povolení.
