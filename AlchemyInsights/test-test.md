---
title: Chýbajúce výrazy v SharePoint online ukladacieho priestoru výrazov
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
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106441"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Povolenie šifrovania BitLocker v Intune

Politiku ochrany koncových bodov služby Intune možno použiť na konfiguráciu nastavení šifrovania BoitLocker pre Windows podľa popisu v nastaveniach Windowsu10 (a novších) na ochranu zariadení pomocou služby Intune.

Mali by ste vedieť, že mnohé novšie zariadenia so Windows 10 podporujú automatické šifrovanie bitlocker, ktoré sa spúšťa bez použitia politiky MDM. Môže to mať vplyv na aplikáciu politiky, ak sú nakonfigurované iné ako predvolené nastavenia. Ďalšie podrobnosti nájdete v téme Najčastejšie otázky.


Najčastejšie otázky: Ktoré vydania balíka Windows podporujú šifrovanie zariadenia pomocou politiky Endpoint Protection?
A: Nastavenia v politike Ochrany koncových bodov služby Intune sa implementuje pomocou šifrovania BitLocker CSP.  Nie všetky vydania ani zostavy šifrovania BitLocker Windows podporu pre šifrovanie BitLocker. V tejto Windows vydania: Enterprise; Podpora pre Vzdelávacie inštitúcie, Mobile, Mobile Enterprise a Professional (od zostavy 1809 od 1809).




Otázka: Ak už je zariadenie šifrované pomocou šifrovania BitLocker pomocou predvolených nastavení operačného systému pre metódu šifrovania a silu šifrovanej jednotky (XTS-AES-128), použitie politiky s rôznymi nastaveniami automaticky spustí opätovné šifrovanie jednotky s novým nastavením?

Odpoveď: Nie. Ak chcete použiť nové nastavenia šifrovanej jednotky, musí sa jednotka najprv dešifrovať.

Poznámka V zariadeniach zaregistrovaných pomocou funkcie Autopilot sa automatické šifrovanie, ktoré sa uskutoční počas funkcie OOBE, nespúšťa až po vyhodnotení politiky intune, ktorá umožňuje použitie nastavení na základe politiky namiesto predvolených nastavení operačného systému.




Q Ak je zariadenie šifrované v dôsledku aplikácie politiky Intune, bude sa pri odstránení tejto politiky dešifrovať?

A: Odstránenie politiky súvisiacej so šifrovaním NEMÁ za následok dešifrovanie nakonfigurovaných jednotiek.




Otázka: Prečo sa v politike dodržiavania súladu pre Intune zdá, že v mojom zariadení nie je zapnuté šifrovanie BitLocker, ale je to?

A: Nastavenie šifrovania BitLocker povolené v politike dodržiavania súladu pre intune používa klienta Windows stavom zariadenia (DHA). Tento klient meria len stav zariadenia pri spustení. Ak sa teda zariadenie od šifrovania bitLocker dokončilo, služba klienta DHA nezadá šifrovanie bitLocker ako aktívne.