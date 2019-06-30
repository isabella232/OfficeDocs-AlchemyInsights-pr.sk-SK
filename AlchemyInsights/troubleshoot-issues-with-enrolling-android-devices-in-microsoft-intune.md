---
title: Riešenie problémov s zapísať Android zariadení Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367304"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Riešenie problémov s zapísať Android zariadení Microsoft Intune

Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz.
  
Niektoré spoločné problémy a rozlíšenie kroky:
  
 **Zariadenia nie sú šifrované chyba v portáli spoločnosti:** Novšie verzie Androidu, najmä počnúc v7.0, požadovať heslo pri spustení uistite sa, že vaše zariadenie je plne šifrované. Povolenie kódu pin pri spustení alebo plne šifrovanie zariadenia sa spoločné riešenia. Prečítať [Tento dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) pre ďalšie informácie.
  
 **Zariadenia nedokážu skontrolovať pomocou služby Windows Intune alebo Zobraziť ako "Nezdravých" Intune admin konzole:** Niektoré Samsung 4.4 a 5,5 zariadenia môže skontrolovať do služby. Existujú 3 možné riešenia tohto problému:
  
1. Manuálne otvorenie aplikácie portáli spoločnosti Intune, ktorý sa automaticky spustí Synchronizácia zariadenia.

2. Aktualizujte zariadenie na Android 6.0 alebo vyšší.

3. Zakázať riadenie portáli Intune spoločnosti Samsung Smart Manager. Prečítať [Tento dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pre ďalšie podrobnosti o týchto otázkach a uznesenia.

 **Užívateľ licencie typu neplatný** alebo **užívateľské meno nerozpozná chyba:** užívateľ musí prideliť licenciu Windows Intune alebo EMS. Revidovať tieto dokumenty priradiť licenciu prostredníctvom: Office Admin Center alebo Azure portál.
  
Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:
  
1. Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie. Prečítať [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre ďalšie podrobnosti.

2. Prečítať [Tento dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pre zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému.

3. [Naučte sa zapísať Android zariadení Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
