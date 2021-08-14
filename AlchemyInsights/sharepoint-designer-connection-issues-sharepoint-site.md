---
title: SharePoint Problémy s pripojením návrhára
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942040"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problémy s pripojením návrhára 

Ak SharePoint Designer vyskytuje problémy s pripojením k SharePoint lokalitám, vyskúšajte nasledujúce bežné riešenia.

Krok 1: Overte, či SharePoint Designer 2013 aktualizuje [balíkom SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a aktualizáciou [pre SharePoint Designer 2013 z 2. augusta 2016.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Krok 2: Vymažte súbory lokálnej vyrovnávacej pamäte:

1. Zavrite SharePoint Designer 2013.

2. V lokálnom počítači odstráňte všetky súbory nájdené v nasledujúcich priečinkoch.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorte SharePoint Designer 2013 a znova zadajte konto, aby ste videli, či funguje.

Krok 3: [Zapnite moderné overovanie pre Office 2013 v Windows zariadeniach](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Krok 4: Správcovia budú musieť **povoliť** vlastný skript v nastaveniach Centra spravovania pre SharePoint, aby bolo možné SharePoint Designer. Ďalšie [informácie nájdete v téme Povolenie alebo zabránenie vlastnému](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) skriptu.


