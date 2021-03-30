---
title: Tajný kľúč klienta registrácie aplikácie alebo problémy s certifikátom
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
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405333"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="e9530-102">Tajný kľúč klienta registrácie aplikácie alebo problémy s certifikátom</span><span class="sxs-lookup"><span data-stu-id="e9530-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="e9530-103">Končí sa platnosť tajného klienta aplikácie?</span><span class="sxs-lookup"><span data-stu-id="e9530-103">Application client secret expiring?</span></span>

<span data-ttu-id="e9530-104">Bez ohľadu na spôsob vytvorenia zaregistrovanej aplikácie, či už prostredníctvom štandardného registračného procesu na portáli registrácie aplikácií alebo prostredníctvom súhlasu nájomníka vytvoril hlavný názov služby, pred uplynutím platnosti aktuálneho a aktualizovaného v súvisiacom kóde aplikácie je potrebné vytvoriť nový kľúč klienta.</span><span class="sxs-lookup"><span data-stu-id="e9530-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="e9530-105">Maximálna platnosť je 2 roky.</span><span class="sxs-lookup"><span data-stu-id="e9530-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="e9530-106">Pripomíname, že tajná hodnota sa musí zaznamenať, pretože po opustení stránky Registrácie aplikácií na portáli už nebude viditeľná.</span><span class="sxs-lookup"><span data-stu-id="e9530-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="e9530-107">Ďalšie informácie nájdete v téme [Rýchly štart: Registrácia aplikácie na platforme identity Microsoft](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) a Osvedčené postupy pre [platformu identity Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="e9530-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="e9530-108">Ďalšie informácie nájdete v téme [Vytvorenie hlavného hlavného & služby Azure AD na portáli – platforme identity Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="e9530-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
