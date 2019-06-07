---
title: Úrovne povolení v SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760707"
---
# <a name="sharepoint-designer-connection-issues"></a>Problémy s pripojením programu SharePoint Designer 

Ak SharePoint Designer je problémy spojenie na lokality SharePoint, prosím, pokus o nasledujúce spoločné riešenia.

Krok 1: Overte, či je aktualizovaný program SharePoint Designer.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Aktualizácia pre program SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Krok 2: Vymazať lokálne cache súbory

- Zatvorte program SharePoint Designer 2013.

- Na lokálnom počítači, vyhľadajte nasledujúce priečinky odstrániť súbory vo vyrovnávacej pamäti.

- Kliknite na tlačidlo Štart, spustiť a odstrániť všetky súbory nájdené v každej z nižšie umiestnenie.

%AppData%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Otvorte program SharePoint Designer 2013 a zadajte konto znova, aby videli, či to funguje.

Krok 3: [umožniť moderné overenie Office 2013 v zariadení so systémom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Krok 4: Správcovia musieť povoliť vlastné skript na povolenie pripojenia programu SharePoint Designer.

Podrobný postup, príklady a úvah nájdete [Povoliť alebo zakázať vlastný skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


