---
title: DataProtection – BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768832"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolenie šifrovania BitLocker so službou Intune

 Politika ochrany koncového bodu služby Intune sa môže použiť na konfiguráciu nastavení šifrovania šifrovania BitLocker pre zariadenia s Windowsom. Ďalšie informácie nájdete v téme [nastavenia Windowsu 10 (a novšie) na ochranu zariadení pomocou služby Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Mali by ste vedieť, že mnoho novších zariadení s Windowsom 10 podporuje automatické šifrovanie BitLocker, ktoré je spustené bez použitia politiky MDM. Môže to mať vplyv na uplatňovanie politiky v prípade, že nie sú nakonfigurované predvolené nastavenia. Ďalšie podrobnosti nájdete v týchto FAQ.
 
Ďalšie informácie o riešení problémov so šifrovaním BitLocker nájdete [v téme Riešenie problémov s politikami šifrovania BitLocker v službe Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Najčastejšie otázky**

Otázka: ktoré vydania systému Windows podporujú šifrovanie zariadenia pomocou politiky koncového bodu ochrany?<br>
A: nastavenie politiky ochrany koncového bodu služby Intune sa implementuje pomocou [funkcie BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nie všetky vydania ani zostavy Windowsu podporujú funkciu BitLocker CSP. <br><br>

Otázka: ako môže byť funkcia BitLocker povolená v zariadeniach bez nutnosti interakcie koncového používateľa?<br>
A: kým sa splnia potrebné predpoklady, je možné povoliť šifrovanie BitLocker tiché šifrovanie prostredníctvom služby Intune. Pozrite si Podrobnosti o požiadavkách na zariadenie a príklade nastavenie politiky na zapnutie tichého šifrovania v nasledujúcom dokumente: [tiché povolenie šifrovania BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

Otázka: Ak je zariadenie už šifrované pomocou šifrovania BitLocker s použitím predvolených nastavení operačného systému pre metódu šifrovania a pevnosť šifrovania (XTS-AES-128), bude uplatňovať politiku s rôznymi nastaveniami automaticky spustiť opätovné šifrovanie jednotky s novými nastaveniami?<br>
Odpoveď: Nie. Ak chcete použiť nové nastavenie šifrovania, jednotka musí byť najprv dešifrovaná.<br><br>
**Poznámka:** V prípade zariadení, ktoré sa zaregistrovali pomocou funkcie autopilot, sa automatické šifrovanie, ktoré sa vyskytne počas OOBE, nespustí, kým sa vyhodnotí politika služby Intune, ktorá umožňuje použiť nastavenia na základe politiky namiesto predvolených hodnôt operačného systému.
 
Otázka: Ak je zariadenie zašifrované ako dôsledok uplatňovania politiky služby Intune, bude sa dešifrovať pri odstránení tejto politiky?<br>
A: Odstránenie politiky súvisiacej s šifrovaním nespôsobí dešifrovanie jednotiek, ktoré boli nakonfigurované.
 
Otázka: prečo sa v politike zabezpečenia služby Intune zobrazuje, že moje zariadenie nemá zapnutú funkciu BitLocker, dokonca aj napriek tomu, že je?<br>
A: nastavenie šifrovania BitLocker v politike zabezpečenia dodržiavania služby Intune využíva klienta Windows Health Atestation (DHA). Tento klient meria stav zariadenia v čase spúšťania. Ak sa však zariadenie po dokončení šifrovania šifrovania BitLocker nereštartovalo, Služba pre klientov DHA neohlási ako aktívnu funkciu BitLocker.
 
 