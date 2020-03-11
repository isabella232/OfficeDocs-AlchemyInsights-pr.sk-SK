---
title: Použitie možnosti odomknúť odtlačok prsta vo Windowse 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588330"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Použitie možnosti odomknúť odtlačok prsta vo Windowse 10

**Povoliť odtlačok prsta v systéme Windows Hello**

Ak chcete Windows 10 odomknúť pomocou odtlačku prsta, musíte nastaviť odtlačok prsta Windows Hello pridaním (nechať Windows naučiť sa rozpoznávať) aspoň jedným prstom. 

1. Prejdite do **časti nastavenia > kontá > možnosti prihlásenia** (alebo kliknite [sem](ms-settings:signinoptions?activationSource=GetHelp)). Dostupné možnosti prihlásenia budú uvedené. Príklad:

    ![Možnosti prihlásenia.](media/sign-in-options.png)

2. Kliknite alebo ťuknite na položku **odtlačok prsta v systéme Windows Hello**a potom kliknite na tlačidlo **nastaviť**. V okne Nastavenie systému Windows Hello kliknite na položku **Začíname**. Snímač odtlačkov prstov sa aktivuje a zobrazí sa výzva na zadanie prsta na senzore:

   ![Snímač odtlačkov prstov.](media/fingerprint-sensor.png)

3. Postupujte podľa pokynov, ktoré vás vyzve, aby ste opakovane skenovať prst. Po dokončení tejto možnosti budete mať možnosť pridať ďalšie prsty, ktoré možno budete chcieť použiť na prihlasovanie. Nabudúce sa prihlásite do systému Windows 10, budete mať možnosť pomocou odtlačku prsta tak urobiť.

**Odtlačok prsta v systéme Windows Hello nie je k dispozícii ako možnosť prihlásenia**

Ak sa odtlačok prsta v systéme Windows Hello nezobrazuje ako možnosť v **možnostiach prihlásenia**, znamená to, že systém Windows nevie o žiadnej čítačke/skeneri odtlačkov prstov pripojenom k počítaču alebo že systémová politika zabraňuje jej používaniu (Ak napríklad počítač spravuje vaše pracovisko). Riešenie problémov s: 

1. Na paneli úloh vyberte tlačidlo **Štart** a vyhľadajte položku **Správca zariadení**.

2. Kliknutím alebo ťuknutím otvorte **správcu zariadení**.

3. V Správcovi zariadení rozbaľte položku Biometrické zariadenia kliknutím na jeho Chevron.

   ![Biometrických zariadení.](media/biometric-devices.png)

4. Snímač odtlačkov prstov by mal byť uvedený ako biometrické zariadenie, ako je napríklad skener Synaptics WBDI:

   ![Biometrických zariadení.](media/biometric-devices-expanded.png)

5. Ak sa skener odtlačkov prstov nezobrazuje a skener je integrovaný do počítača, prejdite na webovú lokalitu výrobcu počítača. V časti Technická podpora pre model počítača vyhľadajte ovládač pre systém Windows 10 pre skener, ktorý môžete nainštalovať.

6. Ak je skener oddelený od počítača (pripojeného cez USB), prejdite na webovú lokalitu výrobcu skenera a vyhľadajte a nainštalujte softvér ovládača zariadenia Windows 10 pre model skenera, ktorý máte.
