---
title: Riešenie problému s PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330974"
---
# <a name="troubleshoot-prt-issue"></a>Riešenie problému s PRT

Aby bolo každé zariadenie dokončené na overenie, musí byť plne zaregistrované a v dobrom stave a môže získať hlavný obnovovací token (PRT).

Proces registrácie hybridného pripojenia k službe Azure AD vyžaduje, aby zariadenia boli v podnikovej sieti. Funguje aj cez sieť VPN, existuje však niekoľko upozornenií. Vypočuli sme zákazníkov, ktorí potrebujú pomoc pri riešení problémov s procesom registrácie hybridného pripojenia k službe Azure AD v prípade okolností na diaľku. Tu je prehľad toho, čo sa deje "pod zákuťom" počas procesu registrácie.

**Prostredie overovania cloudu (pomocou synchronizácie hash hesiel Azure AD alebo odovzdávaného overovania)**

Tento registračný postup je známy aj ako Synchronizácia spojenia.

1. Windows 10 záznam SCP pri prihlásení používateľa do zariadenia.
    1. Zariadenie sa najprv pokúsi načítať informácie nájomníka z kľúča SCP na strane klienta v databáze Registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Ďalšie informácie nájdete v tomto [dokumente.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Ak je pokus neúspešný, zariadenie bude komunikovať s lokálnym prostredím Active Directory (AD) a získať informácie o nájomníkovi z bodu pripojenia služby (SCP). Ak chcete overiť SCP, pozrite si tento [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

**Poznámka:** Odporúčame povoliť SCP v službe AD a na počiatočné overenie použiť iba SCP na strane klienta.

2. Windows 10 sa pokúša komunikovať so službou Azure AD v rámci kontextu systému a overiť sa v službe Azure AD. Pomocou skriptu Test registrácie pripojenia k zariadeniu môžete overiť, či má zariadenie prístup k zdrojom spoločnosti Microsoft v rámci systémového konta.

3. Windows 10 vygeneruje certifikát s vlastným podpisom a uloží ho pod objekt počítača v lokálnej službe AD. Vyžaduje to viditeľnosť radiča domény.

4. Objekt zariadenia s certifikátom sa zosynchronizuje so službou Azure AD prostredníctvom služby Azure AD Pripojenie. Synchronizačný cyklus je predvolene každých 30 minút, ale závisí od konfigurácie služby Azure AD Pripojenie. Ďalšie informácie nájdete v tomto [dokumente.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. V tejto fáze by sa malo pod položkou Blade of Azure Portal zobraziť zariadenie predmetu v stave Čakajúce.

6. Pri prihlásení ďalšieho používateľa do Windows 10 sa registrácia dokončí. 

**Poznámka:** Ak používate sieť VPN a proces prihlásenia pomocou logaff-login ukončí pripojenie domény, registráciu môžete spustiť manuálne:
 1. Problém s dsregcmd /join lokálne v príkazovom riadku správcu alebo vzdialene cez PSExec do počítača. Príklad: PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Ďalšie informácie o problémoch s hybridným pripojením nájdete v téme [Riešenie problémov so zariadeniami.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
