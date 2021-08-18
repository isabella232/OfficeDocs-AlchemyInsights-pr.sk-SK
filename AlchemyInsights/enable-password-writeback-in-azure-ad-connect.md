---
title: Aktivácia spätného zápisu hesiel v službe Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 607e27c883f83b4b29347e764b8f2273cf0f117e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325402"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Aktivácia spätného zápisu hesiel v službe Azure AD Connect

Ak chcete aktivovať spätný zápis samoobslužného resetovania hesla, najskôr aktivujte v službe Azure AD Connect možnosť spätného zápisu. Na serveri Azure AD Connect vykonajte tieto kroky:

1. Prihláste sa na serveri Azure AD Connect a spustite sprievodcu konfiguráciou služby **Azure AD Connect**.
2. Na stránke **Welcome** (Vitajte) kliknite na položku **Next** (Ďalej).
3. Na stránke **Additional tasks** (Ďalšie úlohy) vyberte možnosť **Customize synchronization options** (Prispôsobiť možnosti synchronizácie) a kliknite na položku **Next** (Ďalej).
4. Na stránke **Connect to Azure AD** (Pripojenie k službe AAD) zadajte prihlasovacie údaje globálneho správcu pre nájomníka platformy Azure a kliknite na položku **Next** (Ďalej).
5. Na stránkach **Connect directories** (Pripojenie adresárov) a **Domain/OU filtering** (Filtrovanie domén/organizačných jednotiek) kliknite na položku **Next** (Ďalej).
6. Na stránke **Optional features** (Voliteľné funkcie) začiarknite políčko vedľa možnosti **Password writeback** (Spätný zápis hesiel) a kliknite na položku **Next** (Ďalej).
7. Na stránke **Ready to configure** (Pripravené na konfiguráciu) kliknite na položku **Configure** (Konfigurovať) a počkajte na dokončenie procesu.
8. Keď uvidíte, že sa konfigurácia dokončila, kliknite na možnosť **Exit** (Ukončiť).

Keď máte v službe Azure AD Connect aktivovaný spätný zápis hesiel, nakonfigurujte na spätný zápis Azure AD SSPR.  Ak chcete aktivovať spätný zápis hesiel v službe SSPR, vykonajte tieto kroky:

1. Prihláste sa na portáli Azure použitím konta globálneho správcu.
2. Vyhľadajte a vyberte možnosť **Azure Active Directory**, kliknite na položku **Password reset** (Resetovať heslo) a potom na možnosť **On-premises integration** (Lokálna integrácia).
3. Možnosť **Write back passwords to your on-premises directory?** (Zapisovať heslá spätne do lokálneho adresára?) nastavte na **Yes** (Áno).
4. Možnosť **Allow users to unlock accounts without resetting their password?** (Povoliť používateľom odomykať kontá bez resetovania hesiel?) nastavte na **Yes** (Áno).
5. Keď bude všetko pripravené, kliknite na položku **Save** (Uložiť).

Ďalšie informácie nájdete v téme [Aktivácia spätného zápisu samoobslužného resetovania hesla v službe Azure Active Directory v lokálnom prostredí](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

**Poznámka:** Keď správca obnoví heslo používateľa na portáli Azure, ak je tento používateľ federovaný alebo synchronizovaný hash hesiel, heslo sa zapíše späť do lokálneho systému. Táto funkcia vyžaduje licenciu Azure Premium (P1 alebo P2) a aktuálne ju portál Office Admin nepodporuje
