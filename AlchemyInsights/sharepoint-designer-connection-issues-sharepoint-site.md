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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511559"
---
# <a name="sharepoint-designer-connection-issues"></a>Problémy s pripojením programu SharePoint Designer 

Ak sa v programe SharePoint Designer vyskytli problémy s pripojením na lokality SharePoint, vyskúšajte nasledujúce bežné riešenia.

Krok 1: Overte, či je program SharePoint Designer 2013 aktualizovaný [sharepointovým balíkom Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a aktualizáciou programu [SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)2.



Krok 2: Vymažte lokálne súbory vyrovnávacej pamäte:

1. Zatvorte program SharePoint Designer 2013.

2. Na lokálnom počítači odstráňte všetky súbory nájdené v každom z nasledujúcich priečinkov.

    - %APPDATA%\Microsoft\Rozšírenia webového servera\Vyrovnávacia pamäť
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorte SharePoint Designer 2013 a znova zadajte konto, aby ste zistili, či funguje.

Krok 3: [Povolenie moderného overovania balíka Office 2013 v zariadeniach so systémom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Krok 4: Správcovia budú musieť **povoliť vlastný skript** v nastaveniach Centra spravovania služby SharePoint, aby bolo možné pripojenie programu SharePoint Designer. Ďalšie informácie nájdete v téme [Povolenie alebo zakázanie vlastného skriptu.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


