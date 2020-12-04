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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573907"
---
# <a name="troubleshoot-prt-issue"></a>Riešenie problému s PRT

Ak chcete, aby všetky zariadenia dokončili overenie, musí byť plne zaregistrovaný a v dobrom stave a môže získať primárny token obnovenia (PRT).

Proces registrácie hybridnej Azure AD sa vyžaduje, aby sa zariadenia nachádzali v podnikovej sieti. Funguje aj cez VPN, ale tam sú niektoré námietky na to. Počuli sme zákazníkov, ktorí potrebujú pomoc pri riešení problémov s procesom registrácie hybridnej služby Azure AD v rámci podmienok vzdialenej práce. Tu je rozpis toho, čo sa deje pod kapotou počas procesu registrácie.

**Cloudové overovanie prostredia (pomocou synchronizácie hash hesla služby Azure AD alebo overovacieho overovania)**

Tento registračný tok sa označuje aj ako synchronizačný spoj.

1. Windows 10 zistí záznam SCP pri prihlásení používateľa do zariadenia.
    1. Zariadenie sa najprv pokúsi o načítanie informácií o nájomníkovi z SCP na strane klienta v databáze Registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Ak to zlyhá, zariadenie komunikuje s lokálnou službou Active Directory (AD) na získanie informácií o nájomníkovi z bodu pripojenia služby (SCP). Ak chcete overiť SCP, prečítajte si tento [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Odporúčame povoliť SCP v REKLAMe a len na strane klienta SCP na prvotné overenie.

2. Windows 10 sa pokúša komunikovať so službou Azure AD v rámci systémového kontextu, aby sa overil sám proti službe Azure AD. Ak chcete overiť, či zariadenie môže získať prístup k prostriedkom spoločnosti Microsoft v rámci systémového konta, pomocou skriptu na pripojenie k registrácii testovacieho zariadenia.

3. Windows 10 generuje certifikát s vlastným podpisom a uloží ho pod objekt počítača v lokálnej REKLAMe. Tento postup vyžaduje, aby sa na radiči domény začiarkli.

4. Objekt zariadenia s certifikátom sa synchronizuje so službou Azure AD prostredníctvom služby Azure AD Connect. Cyklus synchronizácie je predvolene každých 30 minút, ale závisí to od konfigurácie služby Azure AD Connect. Ďalšie informácie nájdete v tomto [dokumente](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. V tejto fáze by ste mali mať možnosť Zobraziť predmetové zariadenie v stave čaká sa v časti čepeľ zariadenia na portáli Azure Portal.

6. Pri ďalšom prihlásení používateľa do Windowsu 10 sa registrácia ukončí. 

> [!NOTE]
> Ak sa nachádzate na sieti VPN a proces prihlásenia odhlásenie ukončí pripojenie k doméne, môžete spustiť registráciu manuálne:
 1. Vydať dsregcmd/JOIN lokálne na výzvu správcu alebo vzdialene cez PSExec do počítača. Napríklad PsExec-s \\ win10client01 cmd, dsregcmd/JOIN

 2. Ďalšie informácie o problémoch s hybridným spojením nájdete v téme [Riešenie problémov s zariadeniami](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
