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
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223727"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Obmedzenie prístupu v SharePoint alebo OneDrive

Existuje mnoho spôsobov, ako obmedziť prístup k SharePoint Online/OneDrive služby. Tieto rôzne metódy obmedzenie prístupu sú uvedené nižšie. 

**Povolenie obmedzenie**

SharePoint Online a OneDrive pre podniky, Obmedzujeme prístup položiek lokality, súbory a priečinky, ako iba poskytnutím prístupu pre tie skupiny/jednotlivcov, ktorí by mali mať prístup.

- [Prispôsobiť povolenia pre zoznam SharePoint alebo knižnicu](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prispôsobiť povolenia pre lokalitu SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Zmeniť povolenia na podpriečinok](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrola prístupu z nespravovaná zariadení](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ako SharePoint alebo Office 365 globálne admin, môžete zablokovať alebo obmedziť prístup k obsahu služby SharePoint a OneDrive z nespravovaná zariadení (tie hybridné AD pripojil alebo kompatibilné s Windows Intune).

**Sieťové umiestnenie obmedzenia**

Ako správca IT, môžete ovládať prístup k službe SharePoint a OneDrive zdrojov na základe definovaných sieťových umiestneniach, ktoré dôverujete. To je tiež známy ako umiestnenie-založené politiky. Pre viac informácií, prečítajte si [Kontrola prístupu k SharePoint Online a OneDrive údajov na základe sieťového umiestnenia](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Obmedzenie lokality zámok** 

V rámci SharePoint Online máte možnosť Uzamknúť kolekciu lokalít, takže nikto nemá prístup. Toto sa nastaví pomocou PowerShell a [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocou vlastnosť uzamknutia - [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .

**Obmedziť používateľov od vytvorenia lokalít alebo podlokality**

Ako SharePoint admin alebo Office 365 globálne admin, umožníte používateľom vytvoriť a spravovať vlastné lokality SharePoint, určiť, aký druh stránok môžu vytvárať, a zadajte umiestnenie lokalít. Pre viac informácií, prečítajte si [Vytvorenie spravovať lokality SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

