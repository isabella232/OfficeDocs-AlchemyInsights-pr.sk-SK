---
title: Problémy s výkonom – SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771259"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>Služby SharePoint alebo OneDrive sú pomalé, nedostupné alebo nie sú k dispozícii pre viacerých používateľov

Ak OneDrive alebo SharePoint nie je k dispozícii viacerým používateľom, ktorí mali predtým prístup, môže sa vyskytnúť dočasný problém so službou. [Skontrolujte tabuľu stavu služby](https://portal.office.com/adminportal/home#/servicehealth).

**Pridanie a povolenie používateľa**

Uistite sa, že [priraďujete licencie používateľom v službe Microsoft 365 for Business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Priradenie povolení**

Ak je používateľovi priradená licencia na SharePoint a stále sa zobrazuje hlásenie o odmietnutí prístupu, skontrolujte, či majú priradenú [zodpovedajúcu úroveň povolení](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Zvážte použitie funkcie žiadosť o prístup**

[Funkcia žiadosti o prístup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umožňuje ľuďom požiadať o prístup k obsahu, ktorý momentálne nemajú povolenie na zobrazenie.

**Povolenie vlastného skriptu môže spôsobiť problémy s prístupom k odmietnutým**

K dispozícii sú určité scenáre, v ktorých môže funkcia *Povoliť vlastný skript* prezentovať prístup odmietnutý. Zoznam ovplyvnených funkcií, dôvody zabezpečenia a možnosť vypnutia funkcie. Prejdite na stránku [povolenie alebo zakázanie vlastného skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

