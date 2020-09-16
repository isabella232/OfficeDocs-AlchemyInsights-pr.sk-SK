---
title: Výrazy chýbajúce zo služby SharePoint Online term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750466"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolenie šifrovania BitLocker so službou Intune

Politika ochrany koncového bodu služby Intune sa môže použiť na konfigurovanie nastavení šifrovania Boitlocker pre zariadenia s Windowsom, ako je popísané v téme: windows10 (a novšie verzie) na ochranu zariadení pomocou služby Intune

Mali by ste vedieť, že mnohé novšie zariadenia s Windowsom 10 podporujú automatické šifrovanie šifrovania BitLocker, ktoré je spustené bez použitia politiky MDM. Môže to mať vplyv na uplatňovanie politiky, ak nie sú nakonfigurované iné ako predvolené nastavenia. Ďalšie podrobnosti nájdete v téme Najčastejšie otázky.


FAQ   Q: ktoré vydania systému Windows podporujú šifrovanie zariadenia pomocou politiky koncového bodu ochrany?
 A: nastavenie politiky ochrany koncového bodu služby Intune sa implementuje pomocou funkcie BitLocker CSP.Nie všetky vydania ani zostavy Windowsu nepodporujú funkciu BitLocker CSP. 
      V tejto časovej verzii Windowsu: Enterprise; Podporované sú vzdelávacie, mobilné, mobilné podniky a profesionálna (od zostavy 1809).




Otázka: Ak je zariadenie už šifrované pomocou šifrovania BitLocker s použitím predvolených nastavení operačného systému pre metódu šifrovania a pevnosť šifrovania (XTS-AES-128), bude uplatňovať politiku s rôznymi nastaveniami automaticky spustiť opätovné šifrovanie jednotky s novým nastavením?

Odpoveď: Nie. Ak chcete použiť nové nastavenia šifrovania, jednotka musí byť najprv dešifrovaná.

Poznámka v prípade zariadení, ktoré sa zaregistrovali pomocou funkcie autopilot, automatické šifrovanie, ktoré sa vyskytne počas OOBE, sa nespustí, kým sa nevyhodnotí politika služby Intune, ktorá umožňuje použitie nastavení politiky na mieste predvolených hodnôt operačného systému.




Otázka: Ak je zariadenie zašifrované ako dôsledok uplatňovania politiky služby Intune, po odstránení tejto politiky sa dešifruje?

A: Odstránenie politiky súvisiacej s šifrovaním nevedie k dešifrovaniu jednotiek, ktoré boli nakonfigurované.




Otázka: prečo politika v oblasti dodržiavania súladu so službou Intune zobrazuje, že moje zariadenie nemá zapnutú funkciu BitLocker, ale je to?

A: nastavenie šifrovania BitLocker v politike kompatibility služby Intune využíva klienta Windows Health Atestation (DHA). Tento klient meria stav zariadenia v čase spúšťania. Ak sa už po dokončení šifrovania šifrovania BitLocker nereštartuje zariadenie, klient služby DHA neohlási ako aktívnu funkciu BitLocker.