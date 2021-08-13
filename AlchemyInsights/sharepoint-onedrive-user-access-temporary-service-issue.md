---
title: Problémy s výkonom SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093792"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint alebo OneDrive Slow, Neprístupné alebo Nedostupné pre viacerých používateľov

Ak lokalita OneDrive alebo SharePoint pre viacerých používateľov, ktorí predtým mali prístup, môže ísť o dočasný problém so servisom. [Skontrolujte tabuľu stavu služby.](https://portal.office.com/adminportal/home#/servicehealth)

**Pridanie a licencia pre používateľa**

Uistite [sa, že priradíte licencie používateľom vo Microsoft 365 for business.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Priradenie povolení**

Ak má používateľ priradenú licenciu na SharePoint a stále sa mu zobrazuje hlásenie o odmietnutí prístupu, uistite sa, že má [priradenú príslušnú úroveň](https://docs.microsoft.com/sharepoint/understanding-permission-levels) povolení.

**Zvážte použitie funkcie požiadavky na prístup**

Funkcia [požiadavky na prístup umožňuje](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) používateľom požiadať o prístup k obsahu, ktorý momentálne nemôžu zobraziť.

**Povoliť vlastný skript môže spôsobiť problémy s odmietnutím prístupu**

Existujú určité scenáre, kedy funkcia *Povoliť vlastný skript* môže prezentovať prístup odmietnutý. Zoznam ovplyvnených funkcií, zváženia zabezpečenia a možnosti vypnutia funkcie. Prejdite na [stránku Povolenie alebo zabrá pomôžte predísť vlastnému skriptu.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

