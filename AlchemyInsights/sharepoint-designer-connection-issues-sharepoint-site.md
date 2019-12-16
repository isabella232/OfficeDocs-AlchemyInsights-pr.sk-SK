---
title: Problémy s pripojením programu SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051728"
---
# <a name="sharepoint-designer-connection-issues"></a>Problémy s pripojením programu SharePoint Designer 

Ak SharePoint Designer zažíva problémy s pripojením na lokality SharePoint, vyskúšajte nasledujúce bežné riešenia.

Krok 1: Skontrolujte, či SharePoint Designer 2013 sa aktualizuje [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a [August 2, 2016 aktualizácie programu SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Krok 2: Vymažte lokálne súbory vyrovnávacej pamäte:

1. Zatvorte program SharePoint Designer 2013.

2. V lokálnom počítači odstráňte všetky súbory nájdené v každom z nasledujúcich priečinkov.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorte SharePoint Designer 2013 a zadajte konto znova, aby zistil, či to funguje.

Krok 3: [Povoliť moderné overovanie pre balík Office 2013 v zariadeniach so systémom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Krok 4: Správcovia budú musieť **Povoliť vlastný skript** v nastavení služby SharePoint admin Center povoliť pripojenie programu SharePoint Designer. Ďalšie informácie nájdete v téme [povolenie alebo predchádzanie vlastným skriptom](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


