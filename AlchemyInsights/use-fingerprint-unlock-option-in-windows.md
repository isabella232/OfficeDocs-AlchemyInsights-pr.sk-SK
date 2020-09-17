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
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="40810-102">Používanie možnosti odomknutia odtlačkov prstov vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="40810-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="40810-103">**Povoliť odtlačok prsta Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="40810-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="40810-104">Ak chcete odomknúť Windows 10 pomocou odtlačku prsta, je potrebné nastaviť odtlačok prsta Windows Hello pridaním (ponechanie Windowsu na rozpoznanie) aspoň jedným prstom.</span><span class="sxs-lookup"><span data-stu-id="40810-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="40810-105">Prejdite na **položky nastavenia > kontá > možnosti prihlásenia** (alebo kliknite [sem](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="40810-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="40810-106">Zobrazia sa dostupné možnosti prihlásenia.</span><span class="sxs-lookup"><span data-stu-id="40810-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="40810-107">Príklad:</span><span class="sxs-lookup"><span data-stu-id="40810-107">For example:</span></span>

    ![Možnosti prihlásenia.](media/sign-in-options.png)

2. <span data-ttu-id="40810-109">Kliknite alebo ťuknite na položku **Windows Hello odtlačok prsta**a potom kliknite na položku **nastaviť**.</span><span class="sxs-lookup"><span data-stu-id="40810-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="40810-110">V okne Nastavenie Windows Hello kliknite na položku **Začíname**.</span><span class="sxs-lookup"><span data-stu-id="40810-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="40810-111">Snímač odtlačkov prstov sa aktivuje a zobrazí sa výzva na posunutie prsta na senzor:</span><span class="sxs-lookup"><span data-stu-id="40810-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Snímač odtlačkov prstov.](media/fingerprint-sensor.png)

3. <span data-ttu-id="40810-113">Postupujte podľa pokynov, v ktorých sa zobrazí výzva na opakované prezretie prsta.</span><span class="sxs-lookup"><span data-stu-id="40810-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="40810-114">Po dokončení je možné pridať ďalšie prsty, ktoré možno budete chcieť použiť na prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="40810-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="40810-115">Pri najbližšom prihlásení do Windowsu 10 budete mať možnosť použiť váš odtlačok prsta.</span><span class="sxs-lookup"><span data-stu-id="40810-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="40810-116">**Odtlačok prsta Windows Hello nie je k dispozícii ako možnosť prihlásenia**</span><span class="sxs-lookup"><span data-stu-id="40810-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="40810-117">Ak sa Windows Hello odtlačok prsta nezobrazuje ako možnosť pri **prihlasovaní**, znamená to, že Windows nevie o žiadnej čítačke odtlačkov prstov alebo skeneri pripojenom k vášmu počítaču alebo že systémová politika zabráni jej použitiu (Ak napríklad váš počítač spravuje na pracovisku).</span><span class="sxs-lookup"><span data-stu-id="40810-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="40810-118">Riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="40810-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="40810-119">Na paneli úloh vyberte tlačidlo **Štart** a vyhľadajte položku **Správca zariadení**.</span><span class="sxs-lookup"><span data-stu-id="40810-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="40810-120">Kliknutím alebo ťuknutím otvorte **správcu zariadení**.</span><span class="sxs-lookup"><span data-stu-id="40810-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="40810-121">V Správcovi zariadení rozbaľte položku Biometrické zariadenia kliknutím na jej šípku.</span><span class="sxs-lookup"><span data-stu-id="40810-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrickými zariadeniami.](media/biometric-devices.png)

4. <span data-ttu-id="40810-123">Váš snímač odtlačkov prstov by mal byť uvedený ako biometrické zariadenie, ako napríklad WBDI skener Synaptics:</span><span class="sxs-lookup"><span data-stu-id="40810-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrickými zariadeniami.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="40810-125">Ak sa skener odtlačkov prstov nezobrazuje a skener je integrovaný do počítača, prejdite na webovú lokalitu výrobcu počítača.</span><span class="sxs-lookup"><span data-stu-id="40810-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="40810-126">V časti Technická podpora pre model PC vyhľadajte ovládač Windowsu 10 pre skener, ktorý môžete nainštalovať.</span><span class="sxs-lookup"><span data-stu-id="40810-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="40810-127">Ak je skener oddelený od počítača (pripojeného cez USB), prejdite na webovú lokalitu výrobcu skenera a vyhľadajte a nainštalujte softvér ovládača zariadenia s Windowsom 10 pre model skenera, ktorý používate.</span><span class="sxs-lookup"><span data-stu-id="40810-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
