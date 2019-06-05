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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716906"
---
# <a name="sharepoint-designer-connection-issues"></a>Problémy s pripojením programu SharePoint Designer 

<p>Ak SharePoint Designer je problémy spojenie na lokality SharePoint, prosím, pokus o nasledujúce spoločné riešenia.</p> <p><strong>Krok 1:</strong> <strong>Overenie SharePoint Designer sa aktualizuje&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Aktualizácia pre program SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Krok 2:</strong> <strong>Zrušte lokálne cache súbory</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Zatvorte program SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Na lokálnom počítači, vyhľadajte nasledujúce priečinky odstrániť súbory vo vyrovnávacej pamäti.&nbsp;</li> <li style="font-weight: 400;">Kliknite na tlačidlo <strong>Start -&gt; spustiť</strong> a odstráňte všetky súbory nájdené podľa jednotlivých nižšie umiestnenie.&nbsp;<br /><br />%AppData%\Microsoft\Web server Extensions\Cache<br />%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Otvorte program SharePoint Designer 2013 a zadajte konto znova, aby videli, či to funguje.</li> </ol> <p><strong>Krok 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Umožňujú moderné overenie Office 2013 v zariadení so systémom Windows</strong></a>&nbsp;</p> <p><strong>Krok 4:</strong> <strong>Správcovia bude musieť umožniť vlastné skript na povolenie pripojenia programu SharePoint Designer</strong>.</p> <p>Podrobný postup, príklady a úvah nájdete <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Povoliť alebo zakázať vlastný skript</a>.&nbsp;</p>


