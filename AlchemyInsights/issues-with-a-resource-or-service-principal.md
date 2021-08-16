---
title: Problémy s zdrojom alebo hlavným zdrojom služby
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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028091"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problémy s zdrojom alebo hlavným zdrojom služby

1. Ak ešte len začínate, hlavný názov aplikácie a služby v aplikácii [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) popisuje registráciu aplikácie, objekty aplikácií a istiny služieb v službe Azure Active Directory: čo sú, ako sa používajú a ako navzájom súvisia. Prezentuje sa aj scenár s príkladmi s viacerými nájomníkmi na znázornenie vzťahu medzi objektom aplikácie a zodpovedajúcimi objektmi hlavného objektu služby.
2. Ďalšie informácie o vzťahu medzi aplikáciami a hlavnými objektmi služby nájdete v aplikáciách na čítanie a hlavných [objektoch služby v Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. Postup: Pomocou portálu vytvorte aplikáciu a hlavný názov služby [Azure AD,](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) ktorý má prístup k zdrojom, vám ukáže, ako vytvoriť novú aplikáciu služby Azure Active Directory (Azure AD) a hlavný názov služby, ktorý možno použiť s kontrolou prístupu na základe rolí.
4. Pomocou [hlavného rozhrania API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)služby môžete pomocou programovania spravovať inštancie aplikácií a riadiť činnosti aplikácie v rámci nájomníka.
5. [ServicePrincipal resource type (typ zdrojov v službePrincipal)](https://docs.microsoft.com/graph/api/resources/serviceprincipal) obsahuje zoznam všetkých vlastností a metód pre typ zdroja servicePrincipal.
6. [Rozdiely medzi typmi zdrojov v Azure AD Graph a aplikáciou Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) sa sú dôležité pre rozdiely medzi platformami Azure AD Graph a zdrojmi Graph Microsoft. Zobrazuje zdroje, ktoré majú odlišné názvy alebo nie sú k dispozícii. Tiež zvýrazňuje zdroje dostupné v beta verzii aplikácie Microsoft Graph, ale nie vo verzii v1.0.

**Problémy s hosťovským používateľom**

- Rýchly štart: Pridanie hostí do adresára na [portáli Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) vám ukáže, ako pridať nového hosťa do adresára Azure AD prostredníctvom portálu Azure, odoslať pozvánku a zistiť, ako vyzerá proces na uplatnenie pozvánky hosťa.
- [Kurz: Vytvorenie tokov používateľov v Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) vám ukáže, ako vytvoriť odporúčaný tok používateľov pomocou portálu Azure. Ak hľadáte informácie o nastavení toku hesla vlastníka zdroja (ROPC) v aplikácii, pozrite si článok Konfigurácia toku poverení hesla vlastníka zdroja v službe Azure AD B2C.
