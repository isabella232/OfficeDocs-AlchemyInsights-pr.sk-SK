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
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320137"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Nasadenie Teams ako samostatné alebo pomocou nových alebo existujúcich Office inštalácií

Microsoft Teams je teraz súčasťou nových ***inštalácií balíka*** Aplikácie Microsoft 365 pre veľké organizácie, Aplikácie Microsoft 365 pre podnikateľov a Office pre Mac. Ďalšie informácie nájdete v téme [Kedy Microsoft Teams budú zahrnuté do nových inštalácií balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Okrem toho, počnúc verziou 1906 v aktuálnom kanáli sa Teams pridá do existujúcich inštalácií balíka Aplikácie Microsoft 365 pre veľké organizácie (a Aplikácie Microsoft 365 pre podnikateľov) v zariadeniach so systémom Windows pri aktualizácii existujúcej inštalácie na najnovšiu verziu.  Ďalšie informácie nájdete v téme [A čo sú existujúce inštalácie Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**Poznámka:** Ak nechcete čakať na tento plán nasadenia, môžete nasadiť Teams ako samostatný pre [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) používateľov podľa týchto pokynov alebo môžete používateľov nastaviť tak, aby si Teams nainštalovali sami od spoločnosti [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ak vaša organizácia nie je pripravená na nasadenie Teams, môžete vykonať kroky, [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) pomocou ktoré ***môžete*** Teams z nových alebo [existujúcich](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) inštalácií balíka Office. Ak chcete Teams nainštalovať, ale nechcete, aby sa balík Teams pre používateľa spúšťal automaticky po jeho inštalácii, pozrite si časť Zabránenie automatickému Microsoft Teams [po](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)inštalácii.

Ak ***chcete Teams zariadenia*** so systémom Windows, pozrite si časť [Odinštalovanie Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Ak chcete Microsoft Teams z viacerých cieľových počítačov alebo používateľov, pozrite si [Microsoft Teams nasadenie zariadenia .](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Ak používate zdieľané počítače, služby vzdialenej pracovnej plochy (RDS) alebo VDI (Virtual Desktop Infrastructure), pozrite si časť Zdieľané prostredia počítača a [VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)s Microsoft Teams.

Ak používate e-Office pre Mac, pozrite [si Microsoft Teams inštalácie v Macu.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**Poznámka:** po Teams sa aktualizácie približne každé [dva](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) týždne automaticky aktualizujú novými funkciami a kvalitami. 