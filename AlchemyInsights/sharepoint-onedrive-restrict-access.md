---
title: Obmedzenie prístupu v SharePoint alebo OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735157"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Obmedzenie prístupu v SharePoint alebo OneDrive

Existuje mnoho spôsobov, ako obmedziť prístup k SharePoint Online/OneDrive služby. Tieto rôzne metódy obmedzenie prístupu sú uvedené nižšie. 

Povolenie obmedzenie

SharePoint Online a OneDrive pre podniky, Obmedzujeme prístup položiek lokality, súbory a priečinky, ako iba poskytnutím prístupu pre tie skupiny/jednotlivcov, ktorí by mali mať prístup.

[Prispôsobiť povolenia pre zoznam SharePoint alebo knižnicu](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[Prispôsobiť povolenia pre lokalitu SharePoint](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[Zmeniť povolenia na podpriečinok](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[Kontrola prístupu z nespravovaná zariadení](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

Ako SharePoint alebo Office 365 globálne admin, môžete zablokovať alebo obmedziť prístup k obsahu služby SharePoint a OneDrive z nespravovaná zariadení (tie hybridné AD pripojil alebo kompatibilné s Windows Intune).

Sieťové umiestnenie obmedzenia

Ako správca IT, môžete ovládať prístup k službe SharePoint a OneDrive zdrojov na základe definovaných sieťových umiestneniach, ktoré dôverujete. To je tiež známy ako umiestnenie-založené politiky. Pre viac informácií, prečítajte si [Kontrola prístupu k SharePoint Online a OneDrive údajov na základe sieťového umiestnenia](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)

Obmedzenie lokality zámok 

V rámci SharePoint Online máte možnosť Uzamknúť kolekciu lokalít, takže nikto nemá prístup. Toto sa nastaví pomocou PowerShell a [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocou vlastnosť uzamknutia - [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .

Obmedziť používateľov od vytvorenia lokalít alebo podlokality

Ako SharePoint admin alebo Office 365 globálne admin, umožníte používateľom vytvoriť a spravovať vlastné lokality SharePoint, určiť, aký druh stránok môžu vytvárať, a zadajte umiestnenie lokalít. Pre viac informácií, prečítajte si [Vytvorenie spravovať lokality SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)

