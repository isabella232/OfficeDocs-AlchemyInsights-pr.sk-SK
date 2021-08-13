---
title: Obmedzenie prístupu v SharePoint alebo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093857"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Obmedzenie prístupu v SharePoint alebo OneDrive

Prístup k službám Online/SharePoint alebo OneDrive môžete OneDrive rôznymi spôsobmi. Tieto rôzne metódy obmedzenia prístupu sú uvedené nižšie. 

**Obmedzenie povolení**

V SharePoint Online a OneDrive for Business prístup k položkám, ako sú lokality, súbory a priečinky, obmedzujeme tým, že udelíme prístup len tým skupinám alebo jednotlivcom, ktorí by mali mať prístup.

- [Prispôsobenie povolení pre SharePoint zoznamu alebo knižnice](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prispôsobenie SharePoint lokality](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Zmena povolení pre podpriečinok](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Riadenie prístupu z nespravovaných zariadení](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Ako správca služby SharePoint alebo globálny správca môžete zablokovať alebo obmedziť prístup k obsahu v službe SharePoint a OneDrive z nespravovaných zariadení (tie, ktoré nie sú spojené hybridnou AD alebo kompatibilné v intune).

**Obmedzenie sieťového umiestnenia**

Ako správca IT môžete riadiť prístup k informáciám o SharePoint a OneDrive na základe definovaných sieťových umiestnení, ktoré dôverujete. Táto politika je známa aj ako politika založená na umiestnení. Ďalšie informácie nájdete v téme Riadenie [prístupu k údajom SharePoint Online OneDrive na základe sieťového umiestnenia](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Obmedzenie uzamknutia lokality** 

V SharePoint online máte možnosť uzamknúť kolekciu lokalít, aby k nim mal prístup nikto. Toto sa nastaví prostredníctvom prostredia PowerShell [a SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomocou vlastnosti [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Obmedzenie vytvárania lokalít alebo podlokality používateľmi**

Ako správca služieb SharePoint alebo globálny správca môžete svojim používateľom overiť, či môžu vytvárať a spravovať svoje vlastné lokality služieb SharePoint, určovať druh vytváraných lokalít a určovať umiestnenie lokalít. Ďalšie informácie nájdete v téme Správa [vytvárania lokalít v SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

