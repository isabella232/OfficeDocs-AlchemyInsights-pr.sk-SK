---
title: Výkon problémy-SharePoint alebo OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719531"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint alebo OneDrive pomalá, neprístupná alebo nedostupná pre viacerých používateľov

Ak lokalitu služby OneDrive alebo SharePoint nie je k dispozícii pre viacerých používateľov, ktorí predtým prístup, môže byť problém pri dočasnej služby. [Kontrola tabuľa stav služby](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Pridať a licencia používateľa

Zabezpečiť, že ste [priradiť licenciu na používateľov balíka Office 365 pre podniky](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Priradenie povolení

Ak používateľ nebola priradená licencia Sharepoint a stále sa zobrazuje hlásenie o odmietnutí prístupu, skontrolujte, či majú [príslušnú úroveň povolení](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) priradené.

## <a name="consider-using-the-access-request-feature"></a>Skúste použiť funkciu prístup žiadosť

[Prístup žiadosť funkcia](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) umožňuje ľuďom požiadať o prístup k obsahu, ktoré v súčasnosti nemajú povolenie na zobrazenie.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Povoliť vlastné skript môže spôsobiť prístup odmietnutý problémov

Existujú určité scenáre, kde funkciu *Povoliť vlastný skript* môže predkladať prístup odmietnutý. Pre zoznam funkcií, ktoré sú postihnuté, zabezpečeniu a možnosť vypnúť funkciu. Prosím, navštívte [Povoliť alebo zakázať vlastný skript](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

