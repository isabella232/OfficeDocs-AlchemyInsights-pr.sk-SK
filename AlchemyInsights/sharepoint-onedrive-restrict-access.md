---
title: Obmedzenie prístupu v SharePointe alebo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700470"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Obmedzenie prístupu v SharePointe alebo OneDrive

Existuje mnoho spôsobov, ako obmedziť prístup k službám SharePoint Online/OneDrive. Tieto rozličné spôsoby obmedzenia prístupu sú uvedené nižšie. 

**Obmedzenie povolenia**

V SharePointe Online a vo OneDrive for Business obmedzíme prístup k položkám, akými sú lokality, súbory a priečinky, iba udelením prístupu k týmto skupinám alebo jednotlivcom, ktorí majú mať prístup.

- [Prispôsobenie povolení pre zoznam alebo knižnicu lokality SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prispôsobenie povolení lokality SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Zmena povolení pre podpriečinok](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Riadenie prístupu z nespravovaných zariadení](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ako správca služby SharePoint alebo globálny správca môžete zablokovať alebo obmedziť prístup k obsahu SharePointu a OneDrivu z nespravovaných zariadení (tie, ktoré nie sú hybridnou REKLAMou, ktoré sa pripojili alebo vyhovujú v službe Intune).

**Obmedzenie sieťového umiestnenia**

Ako správca IT môžete ovládať prístup k zdrojom SharePointu a OneDrivu na základe definovaných sieťových umiestnení, ktorým dôverujete. Toto sa označuje aj ako politika založenej na umiestnení. Ďalšie informácie nájdete v téme [Kontrola prístupu k údajom SharePointu Online a OneDrivu na základe sieťového umiestnenia](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) .

**Obmedzenie uzamknutia lokality** 

V SharePointe Online máte možnosť Uzamknúť kolekciu lokalít, takže nikto nemá prístup. Táto možnosť je nastavená cez prostredie PowerShell a [prostredie správy SharePointu Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocou vlastnosti [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Obmedzenie používateľov na vytváranie lokalít alebo podlokalít**

Ako správca služby SharePoint alebo globálny správca môžete používateľom umožniť vytvárať a spravovať vlastné lokality SharePoint, určiť, aký druh lokalít môžu vytvárať, a určiť umiestnenie lokalít. Ďalšie informácie nájdete [v téme Spravovanie vytvárania lokalít v SharePointe Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

