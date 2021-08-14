---
title: Riešenie problémov s hláseniami o odmietnutí prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: af0bc0215f8feacc28a0b9bdf6b2659778736d669f7a3ff17628401e23d5fb6f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957988"
---
# <a name="troubleshoot-access-denied-messages"></a>Riešenie problémov s hláseniami o odmietnutí prístupu

Ak sa pri pokuse o prehľadávanie lokality SharePoint Online zobrazí hlásenie o odmietnutí prístupu, pozrite si nasledujúce články.

**Pridanie a licencia pre používateľa**

Uistite [sa, že priradíte licencie používateľom vo Microsoft 365 for business.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)

**Priradenie povolení**

Ak má používateľ priradenú licenciu na SharePoint a stále sa mu zobrazuje hlásenie o odmietnutí prístupu, uistite sa, že má [priradenú príslušnú úroveň povolení.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)

**Zvážte použitie funkcie požiadavky na prístup**

Funkcia [požiadavky na](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) prístup umožňuje používateľom požiadať o prístup k obsahu, ktorý momentálne nemôžu zobraziť. 

**Povoliť vlastný skript môže spôsobiť problémy s odmietnutím prístupu**

Existujú určité scenáre, kedy funkcia Povoliť vlastný skript môže prezentovať prístup odmietnutý. Zoznam ovplyvnených funkcií, zváženia zabezpečenia a možnosti vypnutia funkcie. Prejdite na stránku , [povolenie alebo zabránenie vlastnému skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

Poznámka: Ak lokalita OneDrive alebo SharePoint pre viacerých používateľov, ktorí predtým mali prístup, môže ísť o dočasný problém so servisom. [Skontrolujte tabuľu stavu služby.](https://portal.office.com/adminportal/home#/servicehealth)


  

