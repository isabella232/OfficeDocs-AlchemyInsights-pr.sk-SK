---
title: Zariadenie v nevybavenom stave
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330387"
---
# <a name="device-in-pending-state"></a>Zariadenie v nevybavenom stave

**Požiadavky:**

1. Ak nastavujete registráciu zariadenia po prvýkrát, skontrolujte Úvodné informácie o riadení zariadení v službe [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) v ktorých nájdete postup, ako získať zariadenia pod kontrolou Azure AD.
2. Ak svoje zariadenia registrujete priamo do služby Azure AD a zaregistrujete ich do služby Intune, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) musíte sa najskôr ubezpečiť, že ste nakonfigurovali [službu Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) a že licencie máte nastavené.
3. Uistite sa, že máte oprávnenie vykonávať operácie v službe Azure AD a lokálnej službe AD. Nastavenia registrácií zariadení môže spravovať iba globálny správca v službe Azure AD. Okrem toho, ak nastavujete automatické registrácie v lokálnej službe Active Directory, budete musieť byť správcom služby Active Directory a AD FS (ak je to potrebné).

Proces registrácie hybridného pripojenia k službe Azure AD vyžaduje, aby zariadenia boli v podnikovej sieti. Funguje aj cez sieť VPN, existuje však niekoľko upozornenií. Vypočuli sme zákazníkov, ktorí potrebujú pomoc pri riešení problémov s procesom hybridného pripojenia k službe Azure AD v prípade okolností na diaľku.

**Prostredie overovania cloudu (pomocou synchronizácie hash hesiel Azure AD alebo odovzdávaného overovania)**

Tento registračný postup je známy aj ako Synchronizácia spojenia.

Tu je prehľad toho, čo sa stane počas registrácie:

1. Windows 10 služba (SCP) zistí, keď sa používateľ prihlási do zariadenia.

    1. Zariadenie sa najprv pokúsi načítať informácie nájomníka z kľúča SCP na strane klienta v databáze Registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Ďalšie informácie nájdete v [dokumente.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. Ak je pokus neúspešný, zariadenie bude komunikovať s lokálnou active Directory a získať informácie o nájomníkovi od SCP. Ak chcete overiť SCP, pozrite si [tento dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    **Poznámka:** Na úvodné overenie sa odporúča povoliť SCP v službe Active Directory a používať iba SCP na strane klienta.

2. Windows 10 sa pokúša komunikovať so službou Azure AD v rámci kontextu systému a overiť sa v službe Azure AD.

    Pomocou skriptu Test registrácie pripojenia k zariadeniu môžete overiť, či má zariadenie prístup k zdrojom spoločnosti Microsoft v [rámci systémového konta.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 vygeneruje certifikát s vlastným podpisom a uloží ho pod objekt počítača v lokálnej službe Active Directory. Vyžaduje to viditeľnosť radiča domény.

4. Objekt zariadenia s certifikátom sa zosynchronizuje so službou Azure AD prostredníctvom služby Azure AD Pripojenie. Synchronizačný cyklus je predvolene každých 30 minút, ale závisí od konfigurácie služby Azure AD Pripojenie. Ďalšie informácie nájdete v tomto [dokumente.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. V tejto fáze by sa malo pod položkou Blade of Azure Portal zobraziť zariadenie predmetu v stave Čakajúce.

6. Pri prihlásení ďalšieho používateľa do Windows 10 sa registrácia dokončí.

    **Poznámka:** Ak používate sieť VPN, prihlásenie/prihlásenie ukončí pripojenie domény, registráciu môžete spustiť manuálne. Ako na to:
    
    Problém lokálne `dsregcmd /join` v príkazovom riadku správcu alebo na diaľku cez PSExec do počítača.\
    Príklad: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Bežné problémy s registráciou Azure Active Directory nájdete v téme Zariadenia – [najčastejšie otázky.](https://docs.microsoft.com/azure/active-directory/devices/faq)
