---
title: Odinštalovanie alebo vylúčenie tímov z inštalácií balíka Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658236"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="eb320-102">Odinštalovanie alebo vylúčenie tímov z nových alebo existujúcich inštalácií balíka Office</span><span class="sxs-lookup"><span data-stu-id="eb320-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="eb320-103">Microsoft teams je súčasťou aplikácií Microsoft 365 pre podniky, Microsoft 365 Apps for Business a Office pre Mac.</span><span class="sxs-lookup"><span data-stu-id="eb320-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="eb320-104">Pomocou [nástroja na nasadenie balíka Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) môžete vylúčiť tímy z nových inštalácií balíka Office.</span><span class="sxs-lookup"><span data-stu-id="eb320-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="eb320-105">Ak chcete *odinštalovať* tímy zo zariadenia so systémom Windows, pozrite si tému [Odinštalovanie aplikácie Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="eb320-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="eb320-106">Ak chcete vyčistenie aplikácie Microsoft teams z viacerých cieľových počítačov alebo používateľov, pozrite si tému [vyčistenie nasadenia v službe Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="eb320-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="eb320-107">Použite možnosť [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , aby ste zabránili automatickej inštalácii aplikácie Microsoft teams s balíkom Office.</span><span class="sxs-lookup"><span data-stu-id="eb320-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="eb320-108">Ak chcete zabrániť automatickému spusteniu aplikácie Microsoft teams po inštalácii, použite možnosť [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *pred nainštalovaním aplikácie teams*.</span><span class="sxs-lookup"><span data-stu-id="eb320-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="eb320-109">Ak používate Office pre Mac, pozrite si tému [Inštalácia aplikácie Microsoft teams v Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="eb320-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>