---
title: Nasadenie Teams ako samostatné alebo pomocou nových alebo existujúcich Office inštalácií
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102217"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Nasadenie Teams ako samostatné alebo pomocou nových alebo existujúcich Office inštalácií

Microsoft Teams je teraz súčasťou nových ***inštalácií balíka*** Aplikácie Microsoft 365 pre veľké organizácie, Aplikácie Microsoft 365 pre podnikateľov a Office pre Mac. Ďalšie informácie nájdete v téme [Kedy Microsoft Teams budú zahrnuté do nových inštalácií balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Okrem toho sa od verzie 1906 v aktuálnom  kanáli Teams pri aktualizácii existujúcej inštalácie na najnovšiu verziu pridá do existujúcich inštalácií balíka Aplikácie Microsoft 365 pre veľké organizácie (a Aplikácie Microsoft 365 pre podnikateľov) v zariadeniach so systémom Windows. Ďalšie informácie nájdete v téme [A čo sú existujúce inštalácie Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ak nechcete čakať na tento plán nasadenia, môžete nasadiť Teams ako samostatný pre [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) používateľov podľa týchto pokynov alebo môžete používateľov nastaviť tak, aby si Teams sami nainštalovali od spoločnosti [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ak vaša organizácia nie je pripravená na nasadenie služby Teams,  môžeme vykonať kroky, [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) pomocou ktoré môžete Teams z nových alebo [existujúcich](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) inštalácií balíka Office. Ak chcete Teams, ale nechcete, aby sa Teams spúšťal automaticky pre používateľa po jeho inštalácii, pozrite si časť Zabránenie automatickému Microsoft Teams [po](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)inštalácii.

Ak ***chcete Teams zariadenia*** so systémom Windows, pozrite si časť [Odinštalovanie Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Ak chcete Microsoft Teams z viacerých cieľových počítačov alebo používateľov, pozrite si [Microsoft Teams nasadenie zariadenia](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ak používate zdieľané počítače, služby vzdialenej pracovnej plochy (RDS) alebo VDI (Virtual Desktop Infrastructure), pozrite si časť Zdieľané prostredia počítača a [VDI s Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

Ak používate e-Office pre Mac, pozrite [si Microsoft Teams inštalácie v Macu.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Po Teams sa aktualizácie približne každé [dva](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) týždne automaticky aktualizujú novými funkciami a kvalitami. 