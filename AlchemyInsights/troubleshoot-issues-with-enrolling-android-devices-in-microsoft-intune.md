---
title: Riešenie problémov s zaregistrovaním zariadení s Androidom v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008093"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Riešenie problémov s zaregistrovaním zariadení s Androidom v Microsoft Intune

Ak chcete problém vyriešiť, pozrite si zdroje uvedené nižšie.
  
Niektoré bežné problémy a kroky na riešenie:
  
 **Chyba Zariadenia nie je šifrovaná Company Portal:** Novšie verzie Androidu, najmä verzie v7.0, vyžadujú prístupový kód na spustenie, aby bolo zariadenie plne šifrované. Bežnými riešeniami sú zapnutie špendlíka pri spustení alebo úplné šifrovanie zariadenia. Ďalšie [informácie nájdete](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) v tomto dokumente.
  
 Zariadenia sa nedokážu pozrieť do služby Intune alebo sa v správcovskej konzole služby **Intune zobrazujú ako Nepovhodné:** Niektoré zariadenia Samsung 4.4 a 5.5 nemusia službu kontrolovať. K dispozícii sú 3 možné riešenia tohto problému:
  
1. Manuálne otvorte aplikáciu Intune Company Portal, ktorá automaticky spustí synchronizáciu zariadenia.

2. Aktualizujte zariadenie na Android 6.0 alebo jeho vyššiu verziu.

3. Zakážte aplikácii Samsung Smart Manager spravovať Intune Company Portal. V [tomto dokumente](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) nájdete ďalšie podrobnosti o týchto problémoch a riešeniach.

 **Chyba typu používateľskej** licencie Neplatný alebo Meno používateľa sa nerozpoznalo: Používateľovi je potrebné priradiť licenciu na Intune alebo EMS.  Pozrite si tieto dokumenty a priraďte licenciu prostredníctvom: Office spravovania alebo portálu Azure.
  
Ďalšie zdroje informácií na vyriešenie problému:
  
1. Pomocou [portálu na riešenie problémov služby Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) môžete diagnostikovať a vyriešiť bežné zlyhania registrácie. Ďalšie [podrobnosti nájdete](https://docs.microsoft.com/intune/help-desk-operators) v tomto dokumente.

2. V [tomto dokumente](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) sa nachádza zoznam bežných chýb, ktoré bránia registrácii a riešeniam jednotlivých chýb.

3. [Zistite, ako zaregistrovať zariadenia s Androidom vo Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
