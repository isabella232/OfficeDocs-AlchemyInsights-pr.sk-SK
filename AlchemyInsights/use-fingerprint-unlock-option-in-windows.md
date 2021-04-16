---
title: Použitie možnosti odomknutia prsta vo Windowse 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796692"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Použitie možnosti odomknutia prsta vo Windowse 10

**Zapnutie odtlačku prsta vo Windows Hello**

Ak chcete Windows 10 odomknúť pomocou odtlačku prsta, je potrebné nastaviť odtlačok prsta Windows Hello pridaním aspoň jedného prsta (ktorý Windows rozpozná, aby ho rozpoznal). 

1. Prejdite na **položky > Kontá > Možnosti prihlásenia** (alebo kliknite [sem](ms-settings:signinoptions?activationSource=GetHelp)). Zobrazí sa zoznam dostupných možností prihlásenia. Príklad:

    ![Možnosti prihlásenia.](media/sign-in-options.png)

2. Kliknite alebo ťuknite na **položku Odtlačok prsta vo Windows Hello** a potom kliknite na položku **Nastaviť**. V okne nastavenia funkcie Windows Hello kliknite na **položku Začíname.** Aktivuje sa senzor odtlačku prsta a zobrazí sa výzva, aby ste na senzor umiestnili prst:

   ![Senzor odtlačku prsta.](media/fingerprint-sensor.png)

3. Postupujte podľa pokynov, ktoré vás požiadajú, aby ste opakovane skenovali prst. Po dokončení tejto úlohy budete mať možnosť pridať ďalšie prsty, ktoré možno budete chcieť použiť na prihlásenie. Keď sa nabudúce prihlásite do Windowsu 10, budete mať možnosť použiť na to odtlačky prsta.

**Odtlačok prsta vo Windows Hello nie je k dispozícii ako možnosť prihlásenia**

Ak sa odtlačky prsta vo Windows Hello nezobrazuje ako možnosť v možnostiach **prihlásenia,** znamená to, že Windows nevie o žiadnom čítačke odtlačkov prsta alebo skeneri pripojenom k PC alebo že systémová politika bráni jeho pracovisku (ak napríklad počítač spravuje vaše pracovisko). Riešenie problémov: 

1. Na paneli **úloh** vyberte tlačidlo Štart a vyhľadajte položku **Správca zariadení**.

2. Kliknutím alebo ťuknutím otvorte Správcu **zariadení**.

3. V Správcovi zariadení rozbaľte položku Biometrické zariadenia kliknutím na jej výložku.

   ![Biometrické zariadenia.](media/biometric-devices.png)

4. Váš skener odtlačkov prsta by mal byť uvedený ako biometrické zariadenie, ako je napríklad Skener WBDI, a tento skener:

   ![Biometrické zariadenia.](media/biometric-devices-expanded.png)

5. Ak sa skener odtlačkov prstov nezobrazuje a skener je integrovaný do počítača, prejdite na webovú lokalitu výrobcu počítača. V časti technickej podpory pre model vášho PC vyhľadajte ovládač pre Windows 10, ktorý môžete nainštalovať.

6. Ak je skener oddelený od PC (pripojeného cez USB), prejdite na webovú lokalitu výrobcu skenera a vyhľadajte a nainštalujte softvér ovládača zariadenia s Windowsom 10 pre model skenera, ktorý máte.
