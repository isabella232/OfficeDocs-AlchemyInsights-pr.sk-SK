---
title: Zablokuje ma podmienený prístup s kompatibilným zariadením
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019163"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Zablokuje ma podmienený prístup s kompatibilným zariadením

**Vysoko odporúčané nástroje**

- [Nástroj na riešenie problémov s registráciou](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) zariadenia – komplexný nástroj, ktorý vám pomôže vyriešiť najbežnejšie problémy s registráciou zariadenia.
- [Skript Test Device Registration Connectivity –](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) nástroj, ktorý zabezpečí prístup k koncovým bodom registrácie zariadenia v rámci systémového konta.
- [Skript vyčistenia zariadenia Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – nástroj, ktorý sa používa na hľadanie a spravovanie zastaraných zariadení vo svojom prostredí.

Tu je niekoľko bežných dôvodov, prečo môže podmienený prístup zlyhať  pre kompatibilné zariadenie alebo prečo sa používateľom môže zobraziť hlásenie Z tohto dôvodu sa v rámci požiadavky na prihlásenie do zdroja prideleného organizáciou táto správa nedá získať.

1. **Zariadenie so zariadením MDM nie je v požadovanom stave:**

Overte, či je zariadenie zaregistrované u schváleného poskytovateľa MDM, ako je napríklad Intune, a *či je označený ako kompatibilný.* Ďalšie informácie o intune nájdete v tomto [dokumente.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Ďalšie informácie o dodržiavaní súladu zariadení a služby Intune nájdete v téme Používanie politiky dodržiavania súladu na nastavenie pravidiel pre zariadenia, ktoré [spravujete pomocou služby Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Ak máte problémy s registrácii zariadenia so službou Intune, podrobnosti o riešení problémov nájdete v článku Riešenie problémov s registráciu [zariadenia v spoločnosti Microsoft.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Ak chcete ďalšiu podporu služby Intune, vytvorte žiadosť o podporu. Ak to chcete urobiť, navštívte stránku [pomoci a technickej podpory služby Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Zariadenie nie je pripojené k sieti organizácií:**

Na získanie prístupu k zdrojom organizácie musí byť zariadenie pripojené k sieti organizácie prostredníctvom priameho pripojenia alebo virtuálnej súkromnej siete (VPN) a musí byť tiež pripojené k Azure Active Directory. Ak sa chcete pripojiť k pracovnému zariadeniu k sieti organizácie, pozrite si časť Pripojenie [pracovného zariadenia k sieti organizácie.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Ak chcete zaregistrovať osobné zariadenie/zariadenie BYOD, pozrite si časť Registrácia [osobného zariadenia v sieti organizácie.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Ak chcete overiť, či sa zariadenie pripojilo k sieti, môžete postupovať podľa krokov pre zaregistrované [zariadenia tu](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) alebo v pracovných [zariadeniach tu.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Ak chcete problém vyriešiť pomocou možnosti Sieťové pripojenie organizácie, postupujte podľa pokynov nižšie:

    1. Prihláste sa Windows pomocou svojho pracovného alebo školského konta, napríklad alain@contoso.com.
    2. Pripojenie k sieti vašej organizácie prostredníctvom siete VPN alebo DirectAccess.
    3. Po pripojení zariadenie uzamknite **stlačením kombinácie Windows klávesu s** logom +L.
    4. Odomknite svoje zariadenie pomocou pracovného alebo školského konta a potom sa znova pokúste získať prístup k problematickej aplikácii alebo službe.

Ak sa zobrazí **chybové hlásenie Z tohto miesta** sa nemôžete dostať znova, problém je pravdepodobne na inom mieste.

3. **Operačný systém nie je podporovaný:**

Uistite sa, že používate podporovanej verzie operačného systému vrátane týchto:

- **Windows klient:** Windows 7 alebo novšia verzia

- **Windows Server:** Windows Server 2008 R2 alebo novšia verzia

- **macOS:** macOS X alebo novšia verzia

- **Android a iOS:** Najnovšia verzia mobilných operačných systémov Android a iOS

4. **Webový prehliadač nie je podporovaný:**

Podporované prehliadače nájdete nižšie. Ak chcete používať podporu prehliadača Chrome Windows 1703 alebo novšími verziami, Windows 10 vyžaduje rozšírenie Konta. V prípade aplikácie Edge 85+ je potrebné, aby sa používateľ prihlásil, aby správne odovzdával informácie o dodržiavaní súladu zariadení. Ďalšie podrobnosti nájdete [tu.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8.1**: Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, spravovaný prehliadač Intune, Safari
- **Android**: **Microsoft Edge:** spravovaný prehliadač Intune, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS:** Chrome, Safari

Ďalšie informácie nájdete v časti **Tu nie je k dispozícii správa** a kroky na riešenie [problémov.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
