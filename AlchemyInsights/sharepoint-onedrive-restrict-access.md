---
title: Obmedzenie prístupu v SharePointe alebo OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750679"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Obmedzenie prístupu v SharePointe alebo OneDrive

Existuje mnoho spôsobov, ako obmedziť prístup k službám SharePoint Online/OneDrive. Tieto rôzne metódy obmedzenia prístupu sú uvedené nižšie. 

**Obmedzenie povolení**

V službe SharePoint Online a OneDrive for Business Obmedzujeme prístup k položkám, ako sú lokality, súbory a priečinky, a to iba poskytnutím prístupu k tým skupinám/jednotlivcom, ktorí majú prístup.

- [Prispôsobenie povolení pre zoznam alebo knižnicu lokality SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prispôsobenie povolení lokality SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Zmena povolení pre podpriečinok](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Ovládanie prístupu z nespravovaných zariadení](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ako SharePoint alebo globálny admin v balíku Office 365, môžete blokovať alebo obmedziť prístup k SharePoint a OneDrive obsah z nespravované zariadenia (tie nie hybridné AD pripojil alebo kompatibilné s Intune).

**Obmedzenie sieťového umiestnenia**

Ako správca IT môžete ovládať prístup k prostriedkom služby SharePoint a OneDrive na základe definovaných sieťových umiestnení, ktorým dôverujete. Toto je známe aj ako politika založená na polohe. Ďalšie informácie nájdete [v téme kontrola prístupu k údajom služby SharePoint Online a OneDrive na základe sieťového umiestnenia](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Obmedzenie zámku lokality** 

V rámci služby SharePoint Online máte možnosť Uzamknúť kolekciu lokalít, takže nikto nemá prístup. Toto je nastavené pomocou prostredia PowerShell a [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocou vlastnosť [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Obmedzenie používateľov na vytváranie lokalít alebo podlokalít**

Ako správca lokality SharePoint alebo Office 365 globálny správca, môžete umožniť používateľom vytvárať a spravovať svoje vlastné lokality SharePoint, určiť, aký druh lokalít, ktoré môžu vytvoriť, a určiť umiestnenie lokalít. Ďalšie informácie nájdete [v téme Spravovanie vytvárania lokalít v SharePointe Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

