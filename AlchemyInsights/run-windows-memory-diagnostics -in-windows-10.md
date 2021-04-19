---
title: Spustenie diagnostiky pamäte Windowsu vo Windowse 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826682"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Spustenie diagnostiky pamäte Windowsu vo Windowse 10

Ak Windows a aplikácie v počítači zlyhávajú, zamŕzajú alebo pôsobia nestabilným spôsobom, môže ísť o problém s pamäťou PC (RAM). Môžete spustiť nástroj Diagnostika pamäte Windowsu a zistiť, či sa v počítači nenálili problémy s pamäťou RAM počítača.

Do vyhľadávacieho poľa na paneli úloh zadajte výraz **Diagnostika pamäte** a potom vyberte položku **Diagnostika pamäte systému Windows.** 

Na spustenie diagnostiky musí byť počítač reštartovaný. Máte možnosť okamžite reštartovať (najprv uložte svoju prácu a zatvorte otvorené dokumenty a e-maily) alebo naplánujte spustenie diagnostiky automaticky pri ďalšom reštartovaní počítača:

![Nástroj Windows Diagnostika pamäte](media/windows-memory-diagnostic.png)

Po reštartovaní počítača sa **nástroj Windows Diagnostika pamäte** spustí automaticky. Stav a priebeh sa budú zobrazovať pri spustení diagnostiky a máte možnosť zrušiť diagnostiku stlačením klávesu **ESC** na klávesnici.

Po dokončení diagnostiky sa Windows spustí normálne.
Po reštartovaní sa hneď po reštartovaní zobrazí oznámenie  (vedľa ikony Centrum akcií na paneli úloh), ktoré informuje, či sa našli nejaké chyby pamäte. Príklad:

Tu je ikona Centra akcií: ![Ikona Centra akcií](media/action-center-icon.png) 

A vzorové oznámenie: ![Žiadne chyby pamäte](media/no-memory-errors.png)

Ak ste oznámenie nestihli,  môžete vybrať ikonu Centra  akcií na paneli úloh a zobraziť centrum akcií a zobraziť posúvateľný zoznam oznámení.

Ak chcete skontrolovať podrobné informácie, **do** vyhľadávacieho poľa na paneli úloh zadajte udalosť a potom vyberte položku **Zobrazovač udalostí**. Na **ľavej table** zobrazovača udalostí prejdite na položku **Denníky Windowsu > systému**. Na pravej table si pri pohľade na  stĺpec Zdroj pozrite zoznam nadol, až kým sa nenájde udalosť s hodnotou Source value **MemoryDiagnostics-Results.** Zvýraznite každú takúto udalosť a v poli na karte Všeobecné pod **zoznamom** zobrazte informácie o výsledku.
