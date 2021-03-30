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
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405440"
---
# <a name="api-permissions-and-consent-process"></a>Povolenia rozhrania API a proces súhlasu

Na prístup k údajom v aplikácii Microsoft Graph musí používateľ alebo správca aplikácii udeliť správne povolenia prostredníctvom procesu súhlasu. [Odkaz na povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) obsahuje zoznam povolení priradených ku každej hlavnej množine rozhraní API programu Microsoft Graph. Poskytuje tiež pokyny na používanie povolení.

**Nastavenie alebo aktualizácia hlavného názov služby**

- [Vytvorenie objektu serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – Tento článok vám ukáže, ako vytvoriť nový objekt servicePrincipal.
- Vytvorte na portáli hlavný názov služby [Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) – tento článok vám ukáže, ako vytvoriť novú aplikáciu Azure Active Directory (Azure AD) a hlavný názov služby, ktoré možno použiť s ovládacím prvkov prístupu na základe rolí.
- Hlavné & aplikácií v [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – Tento článok popisuje registráciu aplikácií, objekty aplikácií a hlavné id služieb v službe Azure Active Directory: čo sú to, ako sa používajú a ako navzájom súvisia.

**Pridanie alebo aktualizácia registrácie aplikácie a poskytnutie súhlasu správcu**

- [Vytvorenie registrácie aplikácie](https://docs.microsoft.com/graph/api/application-post-applications) – Tento článok vám ukáže, ako vytvoriť nový objekt aplikácie.
- [Aktualizácia registrácie aplikácie – povolenia rozhrania API](https://docs.microsoft.com/graph/api/application-update) – Tento článok vám ukáže, ako aktualizovať vlastnosti objektu aplikácie.
- [Poskytnúť súhlas správcu](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – na všeobecnú žiadosť o súhlas a súhlas správcu požadujeme, aby správca explicitne udeľuje súhlas.
- [RBAC (beta) –](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) kontajner na správu rolí pre jednotné definície rolí a priradenia rolí pre poskytovateľov rolí Microsoft 365 RBAC, ktorí podporujú viacero hlavných a viacerých rozsahov v rámci jedného priradenia roly. Toto sa líši *od typu zdroja rbacApplication.* Príkladom takéhoto poskytovateľa pre RBAC je Microsoft Intune. Priradenie roly v Intune môže mať pole hlavných používateľov a pole skupín rozsahu. **Vo verzii beta je to znamená, že je stále vo vývoji a neodporúča sa používať vo vývoji.**
