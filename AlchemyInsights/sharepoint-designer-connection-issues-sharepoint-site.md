---
title: Problémy s pripojením programu SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840566"
---
# <a name="sharepoint-designer-connection-issues"></a>Problémy s pripojením programu SharePoint Designer 

Ak SharePoint Designer je problémy spojenie na lokality SharePoint, skúste nasledujúce spoločné riešenia.

Krok 1: Overenie, že je aktualizovaný program SharePoint Designer 2013 [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a [2 August 2016 aktualizácie SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Krok 2: Vymazať lokálne cache súbory:

1. Zatvorte program SharePoint Designer 2013.

2. Na lokálnom počítači, odstráňte všetky súbory nájdené v každej z nasledujúcich priečinkov.

    - %AppData%\Microsoft\Web server Extensions\Cache
    - %AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorte program SharePoint Designer 2013 a zadajte konto znova, aby videli, či to funguje.

Krok 3: [umožniť moderné overenie Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Krok 4: Správcovia musieť **Povoliť vlastné skript** v SharePoint Admin Center nastavenia na povolenie pripojenia programu SharePoint Designer. Vidieť [Povoliť alebo zakázať vlastný skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) pre viac informácií.


