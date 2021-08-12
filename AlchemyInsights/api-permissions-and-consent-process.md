---
title: Povolenia rozhrania API a proces súhlasu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932076"
---
# <a name="api-permissions-and-consent-process"></a>Povolenia rozhrania API a proces súhlasu

Na prístup k údajom v aplikácii Microsoft Graph musí používateľ alebo správca udeliť správne povolenia prostredníctvom procesu súhlasu. [Microsoft Graph povolení obsahuje](https://docs.microsoft.com/graph/permissions-reference) zoznam povolení priradených ku každej hlavnej množine rozhraní API Microsoft Graph Microsoft. Poskytuje tiež pokyny na používanie povolení.

**Nastavenie alebo aktualizácia hlavného názov služby**

- [Vytvorenie objektu serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – Tento článok vám ukáže, ako vytvoriť nový objekt servicePrincipal.
- Vytvorte na portáli hlavný názov služby [Azure AD pre &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) – Tento článok vám ukáže, ako vytvoriť novú aplikáciu Azure Active Directory (Azure AD) a hlavný názov služby, ktorý možno použiť s ovládacím kontrolou prístupu na základe rolí.
- Hlavný názov služby aplikácií & v [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – Tento článok popisuje registráciu aplikácií, objekty aplikácií a istiny služieb v službe Azure Active Directory: čo sú to, ako sa používajú a ako navzájom súvisia.

**Pridanie alebo aktualizácia registrácie aplikácie a poskytnutie súhlasu správcu**

- [Vytvorenie registrácie aplikácie](https://docs.microsoft.com/graph/api/application-post-applications) – Tento článok vám ukáže, ako vytvoriť nový objekt aplikácie.
- [Aktualizácia registrácie aplikácie – povolenia rozhrania API](https://docs.microsoft.com/graph/api/application-update) – Tento článok vám ukáže, ako aktualizovať vlastnosti objektu aplikácie.
- [Poskytnúť súhlas správcu](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – na všeobecnú žiadosť o súhlas a súhlas správcu požadujeme, aby správca explicitne udeľuje súhlas.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – kontajner na správu rolí pre zjednotené definície rolí a priradenia rolí pre poskytovateľov rolí Microsoft 365 ktorí podporujú viacero hlavných a viacerých rozsahov v rámci jedného priradenia roly. Toto sa líši *od typu zdroja rbacApplication.* Microsoft Intune ako príklad takéhoto poskytovateľa pre prebac. Priradenie roly v Intune môže mať pole hlavných používateľov a pole skupín rozsahu. **Vo verzii beta je to znamená, že je stále vo vývoji a neodporúča sa používať vo vývoji.**
