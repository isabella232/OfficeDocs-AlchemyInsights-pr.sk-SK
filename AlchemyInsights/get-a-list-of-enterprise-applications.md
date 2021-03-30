---
title: Získanie zoznamu podnikových aplikácií
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405513"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="886bd-102">Získanie zoznamu podnikových aplikácií</span><span class="sxs-lookup"><span data-stu-id="886bd-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="886bd-103">Ak chcete získať **zoznam** podnikových aplikácií (všetky aplikácie alebo filtrované podľa zobrazovaného mena, ID, identifikátorov URI identifikátorov atď.) prostredníctvom príkazu v prostredí PowerShell, pozrite si časť [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="886bd-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="886bd-104">Ak chcete získať zoznam hlavných objektov služby (všetky objekty alebo filtrované podľa ID) prostredníctvom príkazu v prostredí Powershell, pozrite si časť [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="886bd-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="886bd-105">Ak chcete zobraziť **zoznam aplikácií nakonfigurovaných na použitie s jazykom SAML, môžu** vám pomôcť nasledujúce skripty prostredia PowerShell:</span><span class="sxs-lookup"><span data-stu-id="886bd-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="886bd-106">Každá aplikácia je to aplikácia OAuth alebo aplikácia SAML (galéria aj aplikácie mimo galérie) by v službe AAD vytvorili dva objekty v prípade ich registrácie.</span><span class="sxs-lookup"><span data-stu-id="886bd-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="886bd-107">Jeden sa nazýva Objekt aplikácie a druhý objekt Service Principal .</span><span class="sxs-lookup"><span data-stu-id="886bd-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="886bd-108">Keď pomocou prostredia PowerShell zanecháte vlastnosti hlavného objektu služby, zistíte, že ku každej aplikácii je priradený určitý počet značiek, napríklad:</span><span class="sxs-lookup"><span data-stu-id="886bd-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="886bd-109">Aplikácie OAuth by mali značku s názvom **WindowsAzureActiveDirectoryIntegratedApp**</span><span class="sxs-lookup"><span data-stu-id="886bd-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="886bd-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="886bd-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="886bd-111">Aplikácie, ktoré nie sú z galérie, by mali značku s názvom **WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="886bd-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="886bd-112">Preto môžete použiť tieto značky a zistiť, o aký druh aplikácie ide.</span><span class="sxs-lookup"><span data-stu-id="886bd-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="886bd-113">Značka "**WindowsAzureActiveDirectoryIntegratedApp**" je bežná pre všetky typy aplikácií.</span><span class="sxs-lookup"><span data-stu-id="886bd-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="886bd-114">Pomocou nasledujúceho zlomku kódu môžete zobraziť zoznam všetkých aplikácií SAML (galéria aj iné než galéria):</span><span class="sxs-lookup"><span data-stu-id="886bd-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="886bd-115">Ďalšie informácie nájdete v téme [Identifikácia aplikácií s podporou saml v Službe Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="886bd-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="886bd-116">**Iba vyhľadať a zobraziť zoznam webových** aplikácií: Pomocou príkazu uvedeného nižšie získate všetky aplikácie Azure AD s typom aplikácie "Web app/API"</span><span class="sxs-lookup"><span data-stu-id="886bd-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="886bd-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="886bd-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="886bd-118">**Vyhľadanie a zoznam samotných natívnych** aplikácií: Spustite nasledujúci príkaz a získajte všetky natívne klientske aplikácie (počítačové a mobilné zariadenia).</span><span class="sxs-lookup"><span data-stu-id="886bd-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="886bd-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="886bd-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="886bd-120">**Export všetkých registrovaných podrobností o aplikácii Azure AD** do CSV: Nasledujúci príkaz exportuje všetky aplikácie Azure AD s požadovanými podrobnosťami do súboru csv:</span><span class="sxs-lookup"><span data-stu-id="886bd-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="886bd-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="886bd-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="886bd-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="886bd-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="886bd-123">**Potrebujete exportovať zoznam nepoužívaných aplikácií Azure** – zostava auditu</span><span class="sxs-lookup"><span data-stu-id="886bd-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="886bd-124">Azure AD dokáže zobraziť denníky aplikácií až na 30 dní za predpokladu, že máte licenciu na Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="886bd-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="886bd-125">Máte dve možnosti, ako uchovať údaje dlhšie ako 30 dní.</span><span class="sxs-lookup"><span data-stu-id="886bd-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="886bd-126">Rozhrania API na vytváranie [zostáv Azure AD môžete](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) použiť na načítanie údajov pomocou programovania a ich uloženie do databázy.</span><span class="sxs-lookup"><span data-stu-id="886bd-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="886bd-127">Denníky auditu môžete prípadne integrovať do systému SIEM tretej strany.</span><span class="sxs-lookup"><span data-stu-id="886bd-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="886bd-128">Zoznam aplikácií si môžete stiahnuť aj pre všetky aplikácie a vlastnené aplikácie v časti Registrácia aplikácií Azure Active Directory>>Stiahnuť>Všetky aplikácie/Vlastnené aplikácie.</span><span class="sxs-lookup"><span data-stu-id="886bd-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="886bd-129">Ak chcete zobraziť zoznam aplikácií prostredníctvom MS Graphu, pozrite si časť Aplikácie zoznamu [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) a typ zdroja [aplikácie – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="886bd-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
