---
title: Nasadenie tímov ako samostatných alebo s novými alebo existujúcimi inštaláciami balíka Office
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
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617910"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Nasadenie tímov ako samostatných alebo s novými alebo existujúcimi inštaláciami balíka Office

Microsoft Teams je teraz súčasťou ***nových inštalácií*** aplikácií Microsoft 365 pre podniky, aplikácií Microsoft 365 pre podniky a balíka Office pre Mac. Ďalšie informácie sa nachádzajú v téme [Kedy sa budú microsoft teams začať súčasťou nových inštalácií balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Okrem toho, počnúc verziou 1906 v aktuálnom kanáli , tímy sa ***pridajú do existujúcich inštalácií*** aplikácií Microsoft 365 pre podniky (a Microsoft 365 Apps for business) v zariadeniach so systémom Windows pri aktualizácii existujúcej inštalácie na najnovšiu verziu. Ďalšie informácie sa nachádzajú v téme [Čo s existujúcimi inštaláciami balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ak nechcete čakať na tento plán zavádzania, môžete nasadiť tímy ako samostatné pre používateľov [podľa týchto pokynov](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   alebo môžete, aby používatelia nainštalovali tímy od spoločnosti  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ak vaša organizácia nie je pripravená nasadiť tímy, máme kroky, ktoré môžete podniknúť na ***vylúčenie tímu*** z [nových](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) alebo [existujúcich](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) inštalácií balíka Office. Ak chcete, aby sa aplikácie Teams nainštalovali, ale nechcete, aby sa aplikácia Teams po inštalácii automaticky spúšťala pre používateľa, pozrite si tému [Zabránenie automatickému spusteniu služby Microsoft Teams po inštalácii](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Ak chcete ***odinštalovať aplikáciu Teams*** zo zariadenia so systémom Windows, pozrite si tému [Odinštalovanie služby Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Ak chcete vyčistiť službu Microsoft Teams z viacerých cieľových počítačov alebo používateľov, pozrite si tému [Čistenie nasadenia služby Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ak používate zdieľané počítače, služby vzdialenej pracovnej plochy (RDS) alebo infraštruktúru virtuálnej pracovnej plochy (VDI), pozrite si tému [Zdieľané počítače a prostredia VDI so službou Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ak používate Office for Mac, pozrite si [tému Inštalácie služby Microsoft Teams v Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Po nainštalovaní služby Teams sa [automaticky aktualizuje](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) približne každé dva týždne novými funkciami a aktualizáciami kvality. 