---
title: Nasadenie tímov ako samostatných alebo nových alebo existujúcich inštalácií balíka Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: ffa91eaf333792af149feda25f9a377ed591b597
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010233"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Nasadenie tímov ako samostatných alebo nových alebo existujúcich inštalácií balíka Office

Microsoft teams je teraz súčasťou ***nových inštalácií*** Microsoft 365 aplikácií pre podniky, Microsoft 365 aplikácie pre podniky a Office for Mac. Ďalšie informácie nájdete v téme [Kedy budú Microsoft teams začať byť súčasťou nových inštalácií balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Okrem toho Počnúc verziou 1906 v mesačnom kanáli, tímy budú ***pridané do existujúcich inštalácií*** Microsoft 365 aplikácií pre podniky (a Microsoft 365 aplikácie pre podniky) na zariadeniach so systémom Windows pri aktualizácii existujúcej inštalácie na najnovšiu verziu. Ďalšie informácie nájdete v téme [čo sú existujúce inštalácie balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ak nechcete čakať na tento plán zavádzania, môžete nasadiť tímy ako samostatný pre svojich používateľov podľa [týchto pokynov](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) alebo môžete mať vaši používatelia nainštalovať tímy pre seba [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

Ak vaša organizácia nie je pripravená nasadiť tímy, máme kroky, ktoré môžete podniknúť na ***vylúčenie tímov*** z [nových](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) alebo [existujúcich](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) inštalácií balíka Office. Ak chcete, aby boli tímy nainštalované, ale nechcete, aby sa tímy automaticky nezačali po jeho nainštalovaní, pozrite si, ako [zabrániť automatickému spusteniu programu Microsoft teams po inštalácii](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Ak chcete ***odinštalovať tímy*** zo zariadenia so systémom Windows, pozrite si [Odinštalovanie tímov Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Vyčistenie Microsoft teams z viacerých cieľových počítačov alebo používateľov, nájdete [Microsoft teams nasadenie vyčistiť](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ak používate zdieľané počítače, služby vzdialenej pracovnej plochy (RDS) alebo Virtual Desktop Infrastructure (VDI), pozrite si [zdieľaný počítač a prostredie VDI s tímami Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ak používate balík Office for Mac, pozrite si [Microsoft teams inštalácie na Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Po nainštalovaní tímov sa [automaticky aktualizuje](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) približne každé dva týždne novými funkciami a kvalitnými aktualizáciami. 