---
title: Použitie možnosti odomknutia prsta v Windows 10
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971950"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Použitie možnosti odomknutia prsta v Windows 10

**Povoliť Windows Hello odtlačok prsta**

Ak chcete Windows 10 odomknutie pomocou odtlačku prsta, je potrebné nastaviť odtlačok prsta tak Windows Hello, že aspoň Windows prsta pridáte (aby ste ho chceli rozpoznať). 

1. Prejdite na **Nastavenia > Kontá > Možnosti prihlásenia** (alebo kliknite [sem](ms-settings:signinoptions?activationSource=GetHelp)). Zobrazí sa zoznam dostupných možností prihlásenia. Príklad:

    ![Možnosti prihlásenia.](media/sign-in-options.png)

2. Kliknite alebo ťuknite **na Windows Hello odtlačok prsta** a potom kliknite **na položku Nastaviť**. V okne Windows Hello kliknite na položku **Začíname**. Aktivuje sa senzor odtlačku prsta a zobrazí sa výzva, aby ste na senzor umiestnili prst:

   ![Senzor odtlačku prsta.](media/fingerprint-sensor.png)

3. Postupujte podľa pokynov, ktoré vás požiadajú, aby ste opakovane skenovali prst. Po dokončení tejto úlohy budete mať možnosť pridať ďalšie prsty, ktoré možno budete chcieť použiť na prihlásenie. Keď sa najbližšie prihlásite do Windows 10, budete mať možnosť použiť na to odtlačky prsta.

**Windows Hello Odtlačok prsta nie je k dispozícii ako možnosť prihlásenia**

Ak sa možnosť Odtlačok prsta nezobrazuje ako možnosť v časti Možnosti **prihlásenia,** znamená Windows, že spoločnosť Windows nevie o žiadnom čítačke odtlačkov prsta alebo skeneri pripojenom k PC alebo že systémová politika bráni jeho používajte (ak napríklad počítač spravuje vaše pracovisko). Windows Hello Riešenie problémov: 

1. Na paneli **úloh** vyberte tlačidlo Štart a vyhľadajte položku **Správca zariadení**.

2. Kliknutím alebo ťuknutím otvorte Správcu **zariadení**.

3. V Správcovi zariadení rozbaľte položku Biometrické zariadenia kliknutím na jej výložku.

   ![Biometrické zariadenia.](media/biometric-devices.png)

4. Váš skener odtlačkov prsta by mal byť uvedený ako biometrické zariadenie, ako je napríklad Skener WBDI, a tento skener:

   ![Biometrické zariadenia.](media/biometric-devices-expanded.png)

5. Ak sa skener odtlačkov prstov nezobrazuje a skener je integrovaný do počítača, prejdite na webovú lokalitu výrobcu počítača. V časti technickej podpory pre model vášho PC vyhľadajte Windows 10 skener, ktorý môžete nainštalovať.

6. Ak je skener oddelený od PC (pripojeného cez USB), prejdite na webovú lokalitu výrobcu skenera Windows 10 vyhľadajte Windows 10 nainštalujte softvér ovládača zariadenia pre model skenera, ktorý máte.
