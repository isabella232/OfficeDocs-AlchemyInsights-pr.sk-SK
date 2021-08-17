---
title: DataProtection – Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118609"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolenie šifrovania BitLocker v Intune

Politiku ochrany koncových bodov služby Intune možno použiť na konfiguráciu nastavení šifrovania BitLocker pre Windows zariadenia. Ďalšie informácie nájdete v téme nastavenia Windows 10 (a novšie [verzie) na ochranu zariadení pomocou služby Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Okrem politiky Endpoint Protection je k dispozícii aj Zostava šifrovania, ktorá poskytuje podrobnejšie zobrazenie stavu šifrovania zariadení. K tejto zostave môžete získať prístup z portálu MEM v časti Zariadenia **> Monitor** a potom v **časti** Konfigurácia vyberte položku [Šifrovať zostavu](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Ak zistíte, že šifrovanie BitLocker nie je povolené podľa očakávania alebo že profil používaný na povolenie šifrovania BitLocker je v chybovom stave, pozrite si správu o šifrovaní a získajte ďalšie informácie o tom, prečo sa takéto správanie vyskytuje.

Podrobnosti o tom, ako interpretovať zostavu vrátane rôznych hodnôt stavu šifrovania, nájdete v téme Sledovanie šifrovania [zariadenia pomocou služby Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Mali by ste vedieť, že mnohé novšie zariadenia so Windows 10 podporujú automatické šifrovanie BitLocker, ktoré sa spúšťa bez použitia politiky MDM. Môže to mať vplyv na aplikáciu politiky, ak sú nakonfigurované iné ako predvolené nastavenia. Ďalšie podrobnosti nájdete v týchto najčastejších otázkach.

Informácie o riešení problémov so šifrovaním bitLocker nájdete v téme Riešenie problémov s [politikami šifrovania BitLocker v Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**Najčastejšie otázky**

Otázka: Ktoré vydania balíka Windows podporujú šifrovanie zariadenia pomocou politiky Endpoint Protection?<br>
A: Nastavenia v politike ochrany koncových bodov služby Intune sa implementuje pomocou [šifrovania Bitlocker CSP.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Nie všetky vydania alebo zostavy šifrovania BitLocker Windows podporu pre šifrovanie BitLocker. <br><br>

Otázka: Ako možno šifrovanie BitLocker zapnúť v zariadeniach bez nutnosti interakcie koncových používateľov?<br>
A: Ak sú splnené potrebné predpoklady, je možné povoliť šifrovanie BitLocker "Silent Encryption" cez Intune. Prečítajte si podrobnosti o požiadavkách na zariadenie a vzorových nastaveniach politiky na povolenie ticha šifrovania v tomto dokumente: [Šifrovanie BitLocker bez zobrazenia zvuku](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

Otázka: Ak už je zariadenie šifrované pomocou šifrovania BitLocker pomocou predvolených nastavení operačného systému pre metódu šifrovania a silu šifrovanej jednotky (XTS-AES-128), automaticky sa pomocou politiky s rôznymi nastaveniami automaticky spustí opätovné šifrovanie jednotky s novým nastavením?<br>
Odpoveď: Nie. Ak chcete použiť nové nastavenia šifrovanej položky, jednotka sa musí najprv dešifrovať.<br><br>
**Poznámka:** V prípade zariadení zaregistrovaných pomocou funkcie Autopilot sa automatické šifrovanie, ktoré sa uskutoční počas funkcie OOBE, nespúšťa až po vyhodnocovaní politiky Intune, ktorá umožňuje použitie nastavení na základe politiky namiesto predvolených nastavení operačného systému.
 
Otázka: Bude zariadenie pri odstránení tejto politiky šifrované v dôsledku aplikácie politiky Intune?<br>
A: Odstránenie politiky súvisiacej so šifrovaním NEMÁ za následok dešifrovanie nakonfigurovaných jednotiek.
 
Otázka: Prečo sa v politike dodržiavania súladu služby Intune zdá, že v mojom zariadení nie je šifrovanie BitLocker zapnuté, aj keď je?<br>
A: Nastavenie šifrovania BitLocker povolené v politike dodržiavania súladu pre Intune používa klienta Windows stavu zariadenia (DHA). Tento klient meria len stav zariadenia pri spustení. Ak sa teda od šifrovania BitLocker neukončilo žiadne zariadenie, klientska služba DHA nezadá šifrovanie BitLocker ako aktívne.
 
 