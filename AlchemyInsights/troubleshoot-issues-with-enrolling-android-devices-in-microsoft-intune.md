---
title: Riešenie problémov s zaregistrovaním zariadení s Androidom v službe Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689969"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Riešenie problémov s zaregistrovaním zariadení s Androidom v službe Microsoft Intune

Ak chcete problém vyriešiť, prečítajte si zdroje uvedené nižšie.
  
Niektoré bežné problémy a kroky na riešenie problémov:
  
 **Chyba zariadenia nie je šifrovaná na portáli spoločnosti:** Novšie verzie Androidu, najmä počnúc v 7.0, vyžadujú prístupový kód pri spustení, aby ste sa uistili, že vaše zariadenie je plne zašifrované. Bežné riešenia umožňujú spustenie PIN kódu alebo úplné zašifrovanie zariadenia. Pozrite si [Tento dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) a získajte ďalšie informácie.
  
 **Zariadenia sa nedokážu vrátiť do projektu so službou Intune alebo Zobraziť ako nezdravé v konzole správcu služby Intune:** Niektoré zariadenia Samsung 4,4 a 5,5 sa nemusia vrátiť do služby. K dispozícii sú 3 možné riešenia tohto problému:
  
1. Manuálne otvorte aplikáciu Intune Company Portal, ktorou sa automaticky spustí Synchronizácia zariadenia.

2. Aktualizujte zariadenie na Android 6,0 alebo novšiu verziu.

3. Vypnutie aplikácie Samsung Smart Manager na spravovanie portálu spoločnosti Intune. Pozrite si [Tento dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) a získajte ďalšie podrobnosti o týchto problémoch a rozlíšeniach.

 **Typ licencie používateľa neplatný** alebo **meno používateľa sa nerozpoznala chyba:** používateľ musí mať priradenú licenciu služby Intune alebo EMS. Pozrite si tieto dokumenty a priraďte licenciu: centrum spravovania služieb Office alebo portál Azure.
  
Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:
  
1. Použite [portál na riešenie problémov so službou Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) na diagnostikovanie a riešenie bežných zlyhaní registrácie. Pozrite si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) a získajte ďalšie podrobnosti.

2. Pozrite si [Tento dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) so zoznamom bežných chýb, ktoré zabránia zápisu a rozlíšeniam.

3. [Zistite, ako prihlásiť zariadenia s Androidom v službe Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
