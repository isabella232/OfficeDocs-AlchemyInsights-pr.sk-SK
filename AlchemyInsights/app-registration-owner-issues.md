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
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405320"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="a5931-102">Problémy s vlastníkom registrácie aplikácie</span><span class="sxs-lookup"><span data-stu-id="a5931-102">App Registration Owner issues</span></span>

<span data-ttu-id="a5931-103">Nižšie sú uvedené dostupné metódy na pridanie istiny ako vlastníkov registrácií aplikácií:</span><span class="sxs-lookup"><span data-stu-id="a5931-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="a5931-104">Používanie modulu Azure AD PowerShell –</span><span class="sxs-lookup"><span data-stu-id="a5931-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="a5931-105">Referencia: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="a5931-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="a5931-106">Používanie Azure CLI – `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="a5931-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="a5931-107">Referencia: [vlastník aplikácie az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="a5931-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="a5931-108">Pomocou MS Graph –</span><span class="sxs-lookup"><span data-stu-id="a5931-108">Using MS Graph -</span></span>

    <span data-ttu-id="a5931-109">Referencia: [Pridanie vlastníka – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="a5931-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="a5931-110">Pomocou portálu Azure AD – prejdite na portal.azure.com [>](https://portal.azure.com/) Azure Active Directory > Registrácia aplikácie > Vyberte aplikáciu > Vlastníci > Pridať vlastníkov</span><span class="sxs-lookup"><span data-stu-id="a5931-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="a5931-111">**Nemôžete zobraziť aplikáciu na aplikácii blade napriek tomu, že ste vlastníkom tejto aplikácie?**</span><span class="sxs-lookup"><span data-stu-id="a5931-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="a5931-112">Vlastník aplikácie nie je administratívnou rolou.</span><span class="sxs-lookup"><span data-stu-id="a5931-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="a5931-113">Ak je povolené nastavenie Obmedziť prístup k portálu [správy Azure AD,](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) aplikácie bude môcť zobraziť len správca na portáli registrácie aplikácií.</span><span class="sxs-lookup"><span data-stu-id="a5931-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="a5931-114">Ak chcete, aby vlastník mohol aplikácie zobrazovať, vypnite toto nastavenie (nastaviť na možnosť NIE) alebo priraďte vlastníkovi rolu správcu iba pre konkrétnu aplikáciu.</span><span class="sxs-lookup"><span data-stu-id="a5931-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="a5931-115">Na tento účely však budete vyžadovať licenciu na Azure AD Premium P2 a povoliť [privilegované spravovanie identite.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="a5931-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
