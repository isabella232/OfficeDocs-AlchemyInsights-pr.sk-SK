---
title: Jak-na-import-nk2-súbory
ms.author: daeite
author: daeite
manager: joallard
ms.date: 5/3/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 1d1b02527c3b614375cf1f84a7a511d9318689b1
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770261"
---
# <a name="how-to-import-nk2-files"></a>Postup na import súborov .nk2 

Pri spustení programu Microsoft Outlook 2013, Outlook 2016, Outlook 2019 alebo Outlook pre Office 365 prvýkrát, vyrovnávacia pamäť pre prezývky (uložené v súbor .nk2 *profilename*) sa importuje do skrytej správe v predvolenom ukladacom priestore správ.

Import súborov .nk2 do programu Outlook 2013, Outlook 2016, Outlook 2019 alebo Outlook pre Office 365, uistite sa, že súbor .nk2 je v nasledujúcom priečinku: %appdata%\Microsoft\Outlook

**Poznámka**: súbor .nk2 musí mať rovnaký názov ako aktuálny profil programu Outlook 2013 alebo 2016 programu Outlook. Predvolene je názov profilu "Outlook." Ak chcete skontrolovať názov profilu, postupujte nasledovne: 
1. Kliknite na tlačidlo **Štart**, a potom kliknite na tlačidlo **Ovládací Panel**.
2. Dvakrát kliknite na **Pošta**.
3. V Nastavenie pošty dialógové okno, vyberte položku **Zobraziť profily**.
4. Vyberte možnosť **Spustiť** > **Spustiť**.
5. Do poľa **Otvoriť** zadajte *outlook.exe /importnk2*a potom kliknite na **tlačidlo OK**. 

Po importe súboru .nk2, obsah súboru sú zlúčené do existujúcich prezývku cache uložených v poštovej schránke.

**Poznámka**: súbor .nk2 premenuje pomocou príponu .old ďalšom spustení programu Outlook 2013, Outlook 2016, Outlook 2019 alebo Outlook pre Office 365. Ak chcete znova importovať súbor .nk2, odstráňte prípony .old súboru prvý.

Ďalšie informácie nájdete v téme [Import alebo kopírovanie zoznamu automatického dokončovania na iný počítač](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).