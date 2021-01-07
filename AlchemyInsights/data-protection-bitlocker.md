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
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778208"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolenie šifrovania BitLocker so službou Intune

Politika ochrany koncového bodu služby Intune sa môže použiť na konfiguráciu nastavení šifrovania šifrovania BitLocker pre zariadenia s Windowsom. Ďalšie informácie nájdete v téme [nastavenia Windowsu 10 (a novšie) na ochranu zariadení pomocou služby Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).

Okrem politiky ochrany koncového bodu je k dispozícii aj správa šifrovania, ktorá poskytuje podrobnejšie zobrazenie stavu šifrovania pre zariadenia. Táto zostava je k dispozícii na portáli MEM v časti **zariadenia > monitor** a potom v časti **Konfigurácia** vyberte položku [Správa šifrovania](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Ak zistíte, že šifrovanie BitLocker nie je povolené podľa očakávaní alebo že profil, ktorý sa používa na povolenie šifrovania BitLocker, sa nachádza v chybovom stave, prečítajte si správu o šifrovaní a Získajte lepšie informácie o tom, prečo sa správanie vyskytuje.

Ak chcete nájsť Podrobnosti o interpretácii zostavy vrátane rôznych hodnôt stavu šifrovania, pozrite si tému [sledovanie šifrovania zariadenia pomocou služby Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).

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
 
 