---
title: Riešenie problémov s zapísať Android zariadenia v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759635"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Riešenie problémov s zapísať Android zariadenia v Microsoft Intune

Prečítajte si nižšie uvedené zdroje a vyriešte problém teraz.
  
Niektoré bežné problémy a kroky riešenia:
  
 **Zariadenie nie je šifrovaná chyba v portáli spoločnosti:** Novšie verzie Androidu, najmä počnúc v 7.0, vyžadujú spúšťací prístupový kód, aby ste sa uistili, že vaše zariadenie je úplne šifrované. Bežné riešenia sú umožňujúce spúšťací kód PIN alebo úplne zašifrovať zariadenie. Ďalšie informácie si prečítajte [v tomto dokumente](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .
  
 **Zariadenia nepodarí overiť pomocou služby Intune alebo Zobraziť ako "nezdravé" v konzole správcu Intune:** Niektoré zariadenia Samsung 4,4 a 5,5 nemusia do služby kontrolovať. Existujú 3 možné riešenia tohto problému:
  
1. Manuálne otvorte aplikáciu Intune Company Portal, ktorá automaticky spustí synchronizáciu zariadenia.

2. Aktualizujte zariadenie na Android 6,0 alebo novší.

3. Zakážte Samsung Smart Manager Spravovanie portálu Intune spoločnosti. Prečítajte si [Tento dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pre ďalšie podrobnosti o týchto otázkach a uzneseniach.

 **Typ licencie používateľa neplatné** alebo **meno používateľa nie je rozpoznaná chyba:** používateľ musí prideliť licenciu Intune alebo EMS. Skontrolujte tieto dokumenty a priraďte licenciu prostredníctvom: Office Admin Center alebo Azure Portal.
  
Ďalšie zdroje, ktoré vám pomôžu vyriešiť váš problém:
  
1. Použite [Intune riešenie problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné registrácie zlyhania. Prečítajte si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre viac informácií.

2. Skontrolujte [Tento dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pre zoznam bežných chýb, ktoré zabraňujú zápisu a rozlíšeniu.

3. [Naučte sa, ako zapísať zariadenia Android v Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
