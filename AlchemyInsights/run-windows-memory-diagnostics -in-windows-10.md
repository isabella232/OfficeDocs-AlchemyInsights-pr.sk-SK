---
title: Spustenie nástroja Windows Diagnostika pamäte v systéme Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358295"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Spustenie nástroja Windows Diagnostika pamäte v systéme Windows 10

Ak systém Windows a aplikácie v počítači zlyhajú, zmrazujú alebo pôsobia nestabilným spôsobom, môže sa stať, že máte problém s pamäťou počítača (RAM). Môžete spustiť Windows Diagnostika pamäte na kontrolu problémov s PC RAM.

Do vyhľadávacieho poľa na paneli úloh zadajte príkaz **Diagnostika pamäte**a potom vyberte položku **Windows Diagnostika pamäte**. 

Ak chcete spustiť diagnostický, PC je potrebné reštartovať. Máte možnosť reštartovať okamžite (prosím uložte svoju prácu a zatvorte otvorené dokumenty a e-maily ako prvý), alebo naplánovať diagnostické spustiť automaticky pri ďalšom reštartovaní počítača:

![Windows Diagnostika pamäte](media/windows-memory-diagnostic.png)

Po reštartovaní počítača sa **nástroj Windows Diagnostika pamäte** spustí automaticky. Stav a priebeh sa zobrazí ako diagnostický beh a máte možnosť zrušiť diagnostiku stlačením klávesu **ESC** na klávesnici.

Po dokončení diagnostiky sa systém Windows spustí normálne.
Ihneď po reštarte, keď sa zobrazí pracovná plocha, zobrazí sa upozornenie (vedľa ikony **centra akcií** na paneli úloh), aby ste uviedli, či sa našli chyby pamäte. Príklad:

Tu je ikona centra akcií: ![Ikona centra akcií](media/action-center-icon.png) 

A vzorové oznámenie: ![Žiadne chyby pamäte](media/no-memory-errors.png)

Ak ste oznámenie vynechali, môžete na paneli úloh vybrať ikonu **centra akcií** , aby sa zobrazil **centrum akcií** a zobrazí sa posúvateľný zoznam upozornení.

Ak chcete skontrolovať podrobné informácie, zadajte **udalosť** do vyhľadávacieho poľa na paneli úloh a potom vyberte položku **Zobrazovač udalostí**. V table **Zobrazovač udalostí**na ľavej strane prejdite na **denníky systému Windows > systém**. Na pravej table prehľadá zoznam pri pohľade na **zdrojový** stĺpec, až uvidíte udalosti s zdrojovú hodnotu **memorydiagnostics-výsledky**. Zvýraznite každú takúto udalosť a pozrite si informácie o výsledku v poli na karte **Všeobecné** pod zoznamom.
