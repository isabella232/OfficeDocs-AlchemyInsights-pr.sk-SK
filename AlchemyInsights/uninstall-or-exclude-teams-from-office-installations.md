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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>Odinštalovanie alebo vylúčenie tímov z nových alebo existujúcich inštalácií balíka Office

Microsoft teams je súčasťou aplikácií Microsoft 365 pre podniky, Microsoft 365 Apps for Business a Office pre Mac.

- Pomocou [nástroja na nasadenie balíka Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) môžete vylúčiť tímy z nových inštalácií balíka Office.
- Ak chcete *odinštalovať* tímy zo zariadenia so systémom Windows, pozrite si tému [Odinštalovanie aplikácie Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Ak chcete vyčistenie aplikácie Microsoft teams z viacerých cieľových počítačov alebo používateľov, pozrite si tému [vyčistenie nasadenia v službe Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- Použite možnosť [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , aby ste zabránili automatickej inštalácii aplikácie Microsoft teams s balíkom Office.
- Ak chcete zabrániť automatickému spusteniu aplikácie Microsoft teams po inštalácii, použite možnosť [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *pred nainštalovaním aplikácie teams*.

Ak používate Office pre Mac, pozrite si tému [Inštalácia aplikácie Microsoft teams v Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).