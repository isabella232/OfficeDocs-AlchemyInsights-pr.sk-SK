---
title: Problémy s vlastníkom registrácie aplikácie
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
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951148"
---
# <a name="app-registration-owner-issues"></a>Problémy s vlastníkom registrácie aplikácie

Nižšie sú uvedené dostupné metódy na pridanie istiny ako vlastníkov registrácií aplikácií:

- Používanie modulu Azure AD PowerShell –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referencia: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Používanie Azure CLI – `az ad app owner add`

    Referencia: [vlastník aplikácie az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Pomocou ms Graph –

    Referencia: [Pridať vlastníka – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Pomocou portálu Azure AD – prejdite na portal.azure.com [>](https://portal.azure.com/) Azure Active Directory > Registrácia aplikácie > Vyberte aplikáciu > Vlastníci > Pridať vlastníkov

**Nemôžete zobraziť aplikáciu na aplikácii blade napriek tomu, že ste vlastníkom tejto aplikácie?**

Vlastník aplikácie nie je administratívnou rolou. Ak je povolené nastavenie Obmedziť prístup k portálu [správy Azure AD,](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) aplikácie bude môcť zobraziť len správca na portáli registrácie aplikácií. Ak chcete, aby vlastník mohol aplikácie zobrazovať, vypnite toto nastavenie (nastaviť na možnosť NIE) alebo priraďte vlastníkovi rolu správcu iba pre konkrétnu aplikáciu. Na tento účely však budete vyžadovať licenciu na Azure AD Premium P2 a povoliť [Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
