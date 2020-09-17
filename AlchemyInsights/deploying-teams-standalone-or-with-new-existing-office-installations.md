---
title: Nasadenie tímov ako samostatných alebo s novými alebo existujúcimi inštaláciami balíka Office
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806774"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Nasadenie tímov ako samostatných alebo s novými alebo existujúcimi inštaláciami balíka Office

Microsoft teams je teraz súčasťou ***nových inštalácií*** aplikácií Microsoft 365 pre podniky, Microsoft 365 Apps for Business a balíka Office pre Mac. Ďalšie informácie nájdete v téme [Kedy sa bude Microsoft teams spúšťať s novými inštaláciami balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Okrem toho Počnúc verziou 1906 v aktuálnom kanáli sa tímy ***pridajú k existujúcim inštaláciám*** aplikácií Microsoft 365 pre podniky (a Microsoft 365 Apps for Business) v zariadeniach s Windowsom, keď aktualizujete existujúcu inštaláciu na najnovšiu verziu. Ďalšie informácie nájdete v téme informácie [o existujúcich inštaláciách balíka Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ak nechcete čakať na tento zavádzací plán, môžete nasadiť tímy ako samostatné pre svojich používateľov podľa [týchto pokynov](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   alebo môžete mať svojich používateľov k dispozícii na inštaláciu tímov  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ak vaša organizácia nie je pripravená na nasadenie aplikácie Teams, máte kroky, ktoré môžete vykonať na ***vylúčenie tímov*** z [nových](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) alebo [existujúcich](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) inštalácií balíka Office. Ak chcete, aby sa aplikácie teams inštalovali, ale nechcete, aby sa po inštalácii spustilo automatické spustenie pre používateľa, pozrite si tému [zabránenie automatickému spusteniu aplikácie Microsoft teams po inštalácii](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Ak chcete ***odinštalovať tímy*** zo zariadenia so systémom Windows, pozrite si tému [Odinštalovanie aplikácie Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Ak chcete vyčistenie aplikácie Microsoft teams z viacerých cieľových zariadení alebo používateľov, pozrite si tému [vyčistenie nasadenia v službe Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ak používate zdieľané počítače, služby Remote Desktop Services (RDS) alebo Virtual Desktop Infrastructure (VDI), pozrite si tému [Zdieľané prostredie v počítačoch a VDI s aplikáciou Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ak používate Office pre Mac, pozrite si tému [Inštalácia aplikácie Microsoft teams v Macu](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Po inštalácii aplikácie teams sa [automaticky aktualizuje](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) približne raz za dva týždne s novými funkciami a aktualizáciami kvality. 