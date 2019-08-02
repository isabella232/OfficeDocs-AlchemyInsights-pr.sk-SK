---
title: Nasadenie tímov ako samostatný alebo nových alebo existujúcich inštalácií balíka Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054245"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Nasadenie tímov ako samostatný alebo nových alebo existujúcich inštalácií balíka Office

Microsoft Teams je teraz zahrnuté ako súčasť ***nových inštaláciách*** Office 365 ProPlus, Office 365 Business a Office for Mac. Ďalšie informácie nájdete v téme [Kedy Microsoft Teams začne byť súčasťou novej inštalácie balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

Navyše, počnúc verziu 1906 v mesačných kanál, tímy bude ***pridaný do existujúcej inštalácie*** Office 365 ProPlus (a Office 365 Business) na zariadeniach so systémom Windows, keď aktualizujete existujúce zariadenie na najnovšiu verziu. Ďalšie informácie nájdete v téme [čo o existujúcej inštalácie balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> Ak nechcete čakať na tento plán zavádzania, môžete nasadiť tímy ako samostatný používateľom podľa [týchto pokynov](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) alebo si môžete používateľom nainštalovať tímy pre seba z [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Ak vaša organizácia nie je pripravený na nasadenie tímov, máme možné kroky na ***vylúčenie tímy*** z [novej](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) alebo [existujúcej](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) inštalácie balíka Office. Ak chcete tímy nainštalované, ale chcem tímy začať automaticky pre používateľa po nainštalovaní, pozri [Zabrániť Microsoft tímy z začína automaticky po inštalácii](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

***Odinštalovať tímy*** zo zariadenia so systémom Windows, pozrite si [Odinštalovať Microsoft tímov](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Vyčistenie Microsoft Teams z viacerých cieľových počítačov alebo používateľov, nájdete [Microsoft tímy nasadenie vyčistiť](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ak používate zdieľané počítače, Remote Desktop Services (RDS) alebo Virtual Desktop Infrastructure (VDI), pozri [zdieľaný počítač a prostrediach VDI s tímami spoločnosti Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ak používate Office pre Mac, pozri [Microsoft tímy zariadenia do Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Po nainštalovaní tímov je [automaticky aktualizovaná](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) približne každé dva týždne s nové funkcie a aktualizácie na zvýšenie kvality. 