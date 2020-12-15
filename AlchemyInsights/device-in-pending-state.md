---
title: Zariadenie v stave čakajúce
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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679991"
---
# <a name="device-in-pending-state"></a>Zariadenie v stave čakajúce

**Predpoklady**

1. Ak nastavujete registráciu zariadenia prvýkrát, skontrolujte, či ste si prezreli [úvodné informácie o správe zariadení v službe Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , ktorá vám poskytne informácie o tom, ako získať zariadenia pod kontrolou služby Azure AD.
2. Ak registrujete zariadenia do služby Azure AD priamo a prihlásite ich do služby Intune, budete musieť zabezpečiť [konfiguráciu služby Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) a mať [licenciu](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) na mieste ako prvý.
3. Uistite sa, že máte oprávnenie vykonávať operácie v službe Azure AD a lokálnu reklamu. Nastavenie registrácií zariadenia môže spravovať len globálny správca v službe Azure AD. Okrem toho, Ak nastavujete automatické registrácie v lokálnej službe Active Directory, budete musieť byť správcom služby Active Directory a AD FS (ak je to možné).

Proces registrácie hybridnej Azure AD sa vyžaduje, aby sa zariadenia nachádzali v podnikovej sieti. Funguje aj cez VPN, ale tam sú niektoré námietky na to. Počuli sme zákazníkov, ktorí potrebujú pomoc pri riešení problémov s procesom registrácie hybridnej služby Azure AD v rámci vzdialenej pracovnej situácie.

**Cloudové overovanie prostredia (pomocou synchronizácie hash hesla služby Azure AD alebo overovacieho overovania)**

Tento registračný tok sa označuje aj ako synchronizačný spoj.

Tu je rozpis toho, čo sa deje počas procesu registrácie:

1. Windows 10 zistí záznam bodu pripojenia služby (SCP), keď sa používateľ prihlási do zariadenia.

    1. Zariadenie sa najprv pokúsi o načítanie informácií o nájomníkovi z SCP na strane klienta v databáze Registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Ďalšie informácie nájdete v téme [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Ak sa to nepodarí, zariadenie komunikuje s lokálnou službou Active Directory na získanie informácií o nájomníkovi z SCP. Ak chcete overiť SCP, prečítajte si tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Odporúčame povoliť SCP v službe Active Directory a použiť len SCP na strane klienta na prvotné overenie.

2. Windows 10 sa pokúša komunikovať so službou Azure AD v rámci systémového kontextu, aby sa overil sám proti službe Azure AD.

    Ak chcete overiť, či zariadenie môže získať prístup k prostriedkom spoločnosti Microsoft v rámci systémového konta, pomocou [skriptu na pripojenie k registrácii testovacieho zariadenia](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 generuje certifikát s vlastným podpisom a uloží ho pod objekt počítača v lokálnej službe Active Directory. Tento postup vyžaduje, aby sa na radiči domény začiarkli.

4. Objekt zariadenia s certifikátom sa synchronizuje so službou Azure AD prostredníctvom služby Azure AD Connect. Cyklus synchronizácie je predvolene každých 30 minút, ale závisí to od konfigurácie služby Azure AD Connect. Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. V tejto fáze by ste mali mať možnosť Zobraziť predmetové zariadenie v stave **čaká** sa v časti čepeľ zariadenia na portáli Azure Portal.

6. Pri ďalšom prihlásení používateľa do Windowsu 10 sa registrácia ukončí.

    > [!NOTE]
    > Ak sa nachádzate na virtuálnej súkromnej sieti a odhlásenie/prihlásenie ukončí pripojenie k doméne, môžete spustiť registráciu manuálne. Ak to chcete urobiť, postupujte nasledovne:
    >
    > Vydá `dsregcmd /join` lokálne na výzvu správcu alebo na diaľku cez PSExec do počítača.
    >
    > Príklad: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Bežné problémy s registráciou zariadenia služby Azure Active Directory nájdete v téme [najčastejšie otázky o zariadeniach](https://docs.microsoft.com/azure/active-directory/devices/faq).
