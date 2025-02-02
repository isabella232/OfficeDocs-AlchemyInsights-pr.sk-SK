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
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116743"
---
# <a name="get-a-list-of-enterprise-applications"></a>Získanie zoznamu podnikových aplikácií

1. Ak chcete získať **zoznam** podnikových aplikácií (všetky aplikácie alebo filtrované podľa zobrazovaného mena, ID, identifikátorov URI identifikátorov atď.) prostredníctvom príkazu v prostredí PowerShell, pozrite si časť [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Ak chcete získať zoznam hlavných objektov služby (všetky objekty alebo filtrované podľa ID) prostredníctvom príkazu v prostredí Powershell, pozrite si časť [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Ak chcete zobraziť **zoznam aplikácií nakonfigurovaných na použitie s jazykom SAML, môžu** vám pomôcť nasledujúce skripty prostredia PowerShell:

    Každá aplikácia je to aplikácia OAuth alebo aplikácia SAML (galéria aj aplikácie mimo galérie) by v službe AAD vytvorili dva objekty v prípade ich registrácie. Jeden sa nazýva Objekt aplikácie a druhý objekt Service Principal . Keď pomocou prostredia PowerShell zanecháte vlastnosti hlavného objektu služby, zistíte, že ku každej aplikácii je priradený určitý počet značiek, napríklad:

    - Aplikácie OAuth by mali značku s názvom **WindowsAzureActiveDirectoryIntegratedApp**
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Aplikácie, ktoré nie sú z galérie, by mali značku s názvom **WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Preto môžete použiť tieto značky a zistiť, o aký druh aplikácie ide. Značka "**WindowsAzureActiveDirectoryIntegratedApp**" je bežná pre všetky typy aplikácií. Pomocou nasledujúceho zlomku kódu môžete zobraziť zoznam všetkých aplikácií SAML (galéria aj iné než galéria):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Ďalšie informácie nájdete v téme [Identifikácia aplikácií s podporou saml v Službe Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Iba vyhľadať a zobraziť zoznam webových** aplikácií: Pomocou príkazu uvedeného nižšie získate všetky aplikácie Azure AD s typom aplikácie "Web app/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Vyhľadanie a zoznam samotných natívnych** aplikácií: Spustite nasledujúci príkaz a získajte všetky natívne klientske aplikácie (počítačové a mobilné zariadenia).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Export všetkých registrovaných podrobností o aplikácii Azure AD** do CSV: Nasledujúci príkaz exportuje všetky aplikácie Azure AD s požadovanými podrobnosťami do súboru csv:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Potrebujete exportovať zoznam nepoužívaných aplikácií Azure** – zostava auditu

    Azure AD dokáže zobraziť denníky aplikácií až na 30 dní za predpokladu, že máte licenciu na Azure AD Premium Ad.
    Máte dve možnosti, ako uchovať údaje dlhšie ako 30 dní. Rozhrania API na vytváranie [zostáv Azure AD môžete](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) použiť na načítanie údajov pomocou programovania a ich uloženie do databázy. Denníky auditu môžete prípadne integrovať do systému SIEM tretej strany.

    Zoznam aplikácií si môžete stiahnuť aj pre všetky aplikácie a vlastnené aplikácie v časti Registrácia aplikácií Azure Active Directory>>Stiahnuť>Všetky aplikácie/Vlastnené aplikácie.

    Zoznam aplikácií prostredníctvom ms Graph nájdete v téme Aplikácie zoznamu [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) a typ prostriedkov [aplikácie – Microsoft Graph v1.0.](https://docs.microsoft.com/graph/api/resources/application)
