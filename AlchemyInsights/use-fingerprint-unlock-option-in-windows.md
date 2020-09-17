---
title: Používanie možnosti odomknutia odtlačkov prstov vo Windowse 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795259"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Používanie možnosti odomknutia odtlačkov prstov vo Windowse 10

**Povoliť odtlačok prsta Windows Hello**

Ak chcete odomknúť Windows 10 pomocou odtlačku prsta, je potrebné nastaviť odtlačok prsta Windows Hello pridaním (ponechanie Windowsu na rozpoznanie) aspoň jedným prstom. 

1. Prejdite na **položky nastavenia > kontá > možnosti prihlásenia** (alebo kliknite [sem](ms-settings:signinoptions?activationSource=GetHelp)). Zobrazia sa dostupné možnosti prihlásenia. Príklad:

    ![Možnosti prihlásenia.](media/sign-in-options.png)

2. Kliknite alebo ťuknite na položku **Windows Hello odtlačok prsta**a potom kliknite na položku **nastaviť**. V okne Nastavenie Windows Hello kliknite na položku **Začíname**. Snímač odtlačkov prstov sa aktivuje a zobrazí sa výzva na posunutie prsta na senzor:

   ![Snímač odtlačkov prstov.](media/fingerprint-sensor.png)

3. Postupujte podľa pokynov, v ktorých sa zobrazí výzva na opakované prezretie prsta. Po dokončení je možné pridať ďalšie prsty, ktoré možno budete chcieť použiť na prihlásenie. Pri najbližšom prihlásení do Windowsu 10 budete mať možnosť použiť váš odtlačok prsta.

**Odtlačok prsta Windows Hello nie je k dispozícii ako možnosť prihlásenia**

Ak sa Windows Hello odtlačok prsta nezobrazuje ako možnosť pri **prihlasovaní**, znamená to, že Windows nevie o žiadnej čítačke odtlačkov prstov alebo skeneri pripojenom k vášmu počítaču alebo že systémová politika zabráni jej použitiu (Ak napríklad váš počítač spravuje na pracovisku). Riešenie problémov: 

1. Na paneli úloh vyberte tlačidlo **Štart** a vyhľadajte položku **Správca zariadení**.

2. Kliknutím alebo ťuknutím otvorte **správcu zariadení**.

3. V Správcovi zariadení rozbaľte položku Biometrické zariadenia kliknutím na jej šípku.

   ![Biometrickými zariadeniami.](media/biometric-devices.png)

4. Váš snímač odtlačkov prstov by mal byť uvedený ako biometrické zariadenie, ako napríklad WBDI skener Synaptics:

   ![Biometrickými zariadeniami.](media/biometric-devices-expanded.png)

5. Ak sa skener odtlačkov prstov nezobrazuje a skener je integrovaný do počítača, prejdite na webovú lokalitu výrobcu počítača. V časti Technická podpora pre model PC vyhľadajte ovládač Windowsu 10 pre skener, ktorý môžete nainštalovať.

6. Ak je skener oddelený od počítača (pripojeného cez USB), prejdite na webovú lokalitu výrobcu skenera a vyhľadajte a nainštalujte softvér ovládača zariadenia s Windowsom 10 pre model skenera, ktorý používate.
