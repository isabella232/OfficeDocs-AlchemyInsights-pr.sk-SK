---
title: Problémy s pripojením v programe SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727186"
---
# <a name="sharepoint-designer-connection-issues"></a>Problémy s pripojením v programe SharePoint Designer 

Ak SharePoint Designer zažíva problémy s pripojením na lokality SharePoint, vyskúšajte tieto bežné riešenia.

Krok 1: overenie, či sa SharePoint Designer 2013 aktualizuje pomocou [služby SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) a [aktualizácie z augusta 2, 2016 pre SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Krok 2: Vymazanie lokálnych súborov vyrovnávacej pamäte:

1. Zatvorenie programu SharePoint Designer 2013.

2. V lokálnom počítači odstráňte všetky súbory nájdené v každom z týchto priečinkov.

    - %APPDATA%\Microsoft\Web server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorte SharePoint Designer 2013 a znova zadajte konto, aby ste zistili, či to funguje.

Krok 3: [povolenie moderného overovania pre Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Krok 4: Správcovia budú musieť **Povoliť vlastné skripty** v nastaveniach centra spravovania služby SharePoint, aby sa umožnilo pripojenie programu SharePoint Designer. Ďalšie informácie nájdete v téme [povolenie alebo zakázanie vlastného skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


