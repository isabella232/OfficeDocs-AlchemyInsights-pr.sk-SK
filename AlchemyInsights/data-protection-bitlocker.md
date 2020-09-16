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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731254"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolenie šifrovania BitLocker so službou Intune

 Politika ochrany koncového bodu služby Intune sa môže použiť na konfiguráciu nastavení šifrovania šifrovania BitLocker pre zariadenia s Windowsom. Ďalšie informácie nájdete v téme [nastavenia Windowsu 10 (a novšie) na ochranu zariadení pomocou služby Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Mali by ste vedieť, že mnoho novších zariadení s Windowsom 10 podporuje automatické šifrovanie BitLocker, ktoré je spustené bez použitia politiky MDM. Môže to mať vplyv na uplatňovanie politiky v prípade, že nie sú nakonfigurované predvolené nastavenia. Ďalšie podrobnosti nájdete v týchto FAQ.
 
Ďalšie informácie o riešení problémov so šifrovaním BitLocker nájdete [v téme Riešenie problémov s politikami šifrovania BitLocker v službe Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Najčastejšie otázky**

 Otázka: ktoré vydania systému Windows podporujú šifrovanie zariadenia pomocou politiky koncového bodu ochrany?<br>
 A: nastavenie politiky ochrany koncového bodu služby Intune sa implementuje pomocou [funkcie BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Nie všetky vydania ani zostavy Windowsu podporujú funkciu BitLocker CSP. <br><br>
      V súčasnosti sú podporované tieto vydania Windowsu: Enterprise, Education, Mobile, Mobile Enterprise a Professional (zostava 1809 a novšia verzia).
 
Otázka: Ak je zariadenie už šifrované pomocou šifrovania BitLocker s použitím predvolených nastavení operačného systému pre metódu šifrovania a pevnosť šifrovania (XTS-AES-128), bude uplatňovať politiku s rôznymi nastaveniami automaticky spustiť opätovné šifrovanie jednotky s novými nastaveniami?<br>
Odpoveď: Nie. Ak chcete použiť nové nastavenie šifrovania, jednotka musí byť najprv dešifrovaná.<br><br>
**Poznámka:** V prípade zariadení, ktoré sa zaregistrovali pomocou funkcie autopilot, sa automatické šifrovanie, ktoré sa vyskytne počas OOBE, nespustí, kým sa vyhodnotí politika služby Intune, ktorá umožňuje použiť nastavenia na základe politiky namiesto predvolených hodnôt operačného systému.
 
Otázka: Ak je zariadenie zašifrované ako dôsledok uplatňovania politiky služby Intune, bude sa dešifrovať pri odstránení tejto politiky?<br>
A: Odstránenie politiky súvisiacej s šifrovaním nespôsobí dešifrovanie jednotiek, ktoré boli nakonfigurované.
 
Otázka: prečo sa v politike zabezpečenia služby Intune zobrazuje, že moje zariadenie nemá zapnutú funkciu BitLocker, dokonca aj napriek tomu, že je?<br>
A: nastavenie šifrovania BitLocker v politike zabezpečenia dodržiavania služby Intune využíva klienta Windows Health Atestation (DHA). Tento klient meria stav zariadenia v čase spúšťania. Ak sa však zariadenie po dokončení šifrovania šifrovania BitLocker nereštartovalo, Služba pre klientov DHA neohlási ako aktívnu funkciu BitLocker.
 
 