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
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="64b6a-102">Povolenia rozhrania API a proces súhlasu</span><span class="sxs-lookup"><span data-stu-id="64b6a-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="64b6a-103">Na prístup k údajom v aplikácii Microsoft Graph musí používateľ alebo správca aplikácii udeliť správne povolenia prostredníctvom procesu súhlasu.</span><span class="sxs-lookup"><span data-stu-id="64b6a-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="64b6a-104">[Odkaz na povolenia programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) obsahuje zoznam povolení priradených ku každej hlavnej množine rozhraní API programu Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="64b6a-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="64b6a-105">Poskytuje tiež pokyny na používanie povolení.</span><span class="sxs-lookup"><span data-stu-id="64b6a-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="64b6a-106">**Nastavenie alebo aktualizácia hlavného názov služby**</span><span class="sxs-lookup"><span data-stu-id="64b6a-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="64b6a-107">[Vytvorenie objektu serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – Tento článok vám ukáže, ako vytvoriť nový objekt servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="64b6a-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="64b6a-108">Vytvorte na portáli hlavný názov služby [Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) – tento článok vám ukáže, ako vytvoriť novú aplikáciu Azure Active Directory (Azure AD) a hlavný názov služby, ktoré možno použiť s ovládacím prvkov prístupu na základe rolí.</span><span class="sxs-lookup"><span data-stu-id="64b6a-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="64b6a-109">Hlavné & aplikácií v [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – Tento článok popisuje registráciu aplikácií, objekty aplikácií a hlavné id služieb v službe Azure Active Directory: čo sú to, ako sa používajú a ako navzájom súvisia.</span><span class="sxs-lookup"><span data-stu-id="64b6a-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="64b6a-110">**Pridanie alebo aktualizácia registrácie aplikácie a poskytnutie súhlasu správcu**</span><span class="sxs-lookup"><span data-stu-id="64b6a-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="64b6a-111">[Vytvorenie registrácie aplikácie](https://docs.microsoft.com/graph/api/application-post-applications) – Tento článok vám ukáže, ako vytvoriť nový objekt aplikácie.</span><span class="sxs-lookup"><span data-stu-id="64b6a-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="64b6a-112">[Aktualizácia registrácie aplikácie – povolenia rozhrania API](https://docs.microsoft.com/graph/api/application-update) – Tento článok vám ukáže, ako aktualizovať vlastnosti objektu aplikácie.</span><span class="sxs-lookup"><span data-stu-id="64b6a-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="64b6a-113">[Poskytnúť súhlas správcu](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) – na všeobecnú žiadosť o súhlas a súhlas správcu požadujeme, aby správca explicitne udeľuje súhlas.</span><span class="sxs-lookup"><span data-stu-id="64b6a-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="64b6a-114">[RBAC (beta) –](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) kontajner na správu rolí pre jednotné definície rolí a priradenia rolí pre poskytovateľov rolí Microsoft 365 RBAC, ktorí podporujú viacero hlavných a viacerých rozsahov v rámci jedného priradenia roly.</span><span class="sxs-lookup"><span data-stu-id="64b6a-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="64b6a-115">Toto sa líši *od typu zdroja rbacApplication.*</span><span class="sxs-lookup"><span data-stu-id="64b6a-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="64b6a-116">Príkladom takéhoto poskytovateľa pre RBAC je Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="64b6a-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="64b6a-117">Priradenie roly v Intune môže mať pole hlavných používateľov a pole skupín rozsahu.</span><span class="sxs-lookup"><span data-stu-id="64b6a-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="64b6a-118">**Vo verzii beta je to znamená, že je stále vo vývoji a neodporúča sa používať vo vývoji.**</span><span class="sxs-lookup"><span data-stu-id="64b6a-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
