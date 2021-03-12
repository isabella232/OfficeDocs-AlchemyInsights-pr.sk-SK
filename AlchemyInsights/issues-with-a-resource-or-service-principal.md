---
title: Problémy s hlavným zdrojom alebo službou
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714085"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problémy s hlavným zdrojom alebo službou

1. Ak práve začínate, [hlavné objekty aplikácií a služieb v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) popisujú registráciu aplikácií, objekty aplikácií a princípy služieb v službe Azure Active Directory: čo sú, ako sa používajú a ako sa navzájom súvisia. Na ilustráciu vzťahu medzi objektom aplikácie aplikácie a zodpovedajúcimi hlavnými objektmi služby je prezentovaný aj príklad scenára s viacerými nájomníkmi.
2. Ďalšie informácie o vzťahoch medzi aplikáciami a princípmi služieb nájdete v téme čítanie [aplikácií a hlavných objektov služby v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Ako na to: použitie portálu na vytvorenie aplikácie Azure AD a hlavné služby, ktoré môžu získať prístup k prostriedkom](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) , vám ukáže, ako vytvoriť novú aplikáciu Azure Active Directory (Azure AD), ktorá môže byť použitá s ovládacím prvkom riadenia prístupu na základe rolí.
4. Pomocou [hlavného rozhrania API služby](https://docs.microsoft.com/graph/api/resources/serviceprincipal)môžete pomocou programovania spravovať inštancie aplikácií a riadiť, čo môže aplikácia vykonávať v rámci vášho nájomníka.
5. [Typ zdroja servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) obsahuje všetky vlastnosti a metódy pre typ zdroja servicePrincipal.
6. [Rozdiely v type zdroja medzi Azure AD graphom a Microsoft graphom](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) zvýrazňujú rozdiely medzi Azure AD Graph a Microsoft Graph Resources. Zobrazuje zdroje, ktoré majú rôzne názvy alebo nie sú k dispozícii; vyzdvihuje tiež zdroje dostupné v beta verzii programu Microsoft Graph, ale nie v verzii v 1.0.

**Problémy s hosťujúcimi používateľmi**

- Rýchly štart [: Pridanie hosťujúcich používateľov do adresára na portáli Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) vám ukáže, ako pridať nového hosťujúceho používateľa do adresára služby Azure AD prostredníctvom portálu Azure, Odoslať pozvánku a zistiť, ako vyzerá proces vyplatenia používateľa hosťa.
- [Kurz: Vytvorenie používateľských tokov v službe Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) vám ukáže, ako vytvoriť niektoré Odporúčané toky používateľov pomocou portálu Azure. Ak hľadáte informácie o tom, ako v aplikácii nastaviť tok údajov vlastníka hesla vlastníka prostriedku (ROPC), prečítajte si tému Konfigurácia toku poverení hesla vlastníka prostriedku v službe Azure AD B2C.
