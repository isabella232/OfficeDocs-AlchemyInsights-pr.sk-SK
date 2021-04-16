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
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="d2086-102">Použitie možnosti odomknutia prsta vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="d2086-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="d2086-103">**Zapnutie odtlačku prsta vo Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="d2086-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="d2086-104">Ak chcete Windows 10 odomknúť pomocou odtlačku prsta, je potrebné nastaviť odtlačok prsta Windows Hello pridaním aspoň jedného prsta (ktorý Windows rozpozná, aby ho rozpoznal).</span><span class="sxs-lookup"><span data-stu-id="d2086-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="d2086-105">Prejdite na **položky > Kontá > Možnosti prihlásenia** (alebo kliknite [sem](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="d2086-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="d2086-106">Zobrazí sa zoznam dostupných možností prihlásenia.</span><span class="sxs-lookup"><span data-stu-id="d2086-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="d2086-107">Príklad:</span><span class="sxs-lookup"><span data-stu-id="d2086-107">For example:</span></span>

    ![Možnosti prihlásenia.](media/sign-in-options.png)

2. <span data-ttu-id="d2086-109">Kliknite alebo ťuknite na **položku Odtlačok prsta vo Windows Hello** a potom kliknite na položku **Nastaviť**.</span><span class="sxs-lookup"><span data-stu-id="d2086-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="d2086-110">V okne nastavenia funkcie Windows Hello kliknite na **položku Začíname.**</span><span class="sxs-lookup"><span data-stu-id="d2086-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="d2086-111">Aktivuje sa senzor odtlačku prsta a zobrazí sa výzva, aby ste na senzor umiestnili prst:</span><span class="sxs-lookup"><span data-stu-id="d2086-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor odtlačku prsta.](media/fingerprint-sensor.png)

3. <span data-ttu-id="d2086-113">Postupujte podľa pokynov, ktoré vás požiadajú, aby ste opakovane skenovali prst.</span><span class="sxs-lookup"><span data-stu-id="d2086-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="d2086-114">Po dokončení tejto úlohy budete mať možnosť pridať ďalšie prsty, ktoré možno budete chcieť použiť na prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="d2086-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="d2086-115">Keď sa nabudúce prihlásite do Windowsu 10, budete mať možnosť použiť na to odtlačky prsta.</span><span class="sxs-lookup"><span data-stu-id="d2086-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="d2086-116">**Odtlačok prsta vo Windows Hello nie je k dispozícii ako možnosť prihlásenia**</span><span class="sxs-lookup"><span data-stu-id="d2086-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="d2086-117">Ak sa odtlačky prsta vo Windows Hello nezobrazuje ako možnosť v možnostiach **prihlásenia,** znamená to, že Windows nevie o žiadnom čítačke odtlačkov prsta alebo skeneri pripojenom k PC alebo že systémová politika bráni jeho pracovisku (ak napríklad počítač spravuje vaše pracovisko).</span><span class="sxs-lookup"><span data-stu-id="d2086-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="d2086-118">Riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="d2086-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="d2086-119">Na paneli **úloh** vyberte tlačidlo Štart a vyhľadajte položku **Správca zariadení**.</span><span class="sxs-lookup"><span data-stu-id="d2086-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="d2086-120">Kliknutím alebo ťuknutím otvorte Správcu **zariadení**.</span><span class="sxs-lookup"><span data-stu-id="d2086-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="d2086-121">V Správcovi zariadení rozbaľte položku Biometrické zariadenia kliknutím na jej výložku.</span><span class="sxs-lookup"><span data-stu-id="d2086-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrické zariadenia.](media/biometric-devices.png)

4. <span data-ttu-id="d2086-123">Váš skener odtlačkov prsta by mal byť uvedený ako biometrické zariadenie, ako je napríklad Skener WBDI, a tento skener:</span><span class="sxs-lookup"><span data-stu-id="d2086-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrické zariadenia.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="d2086-125">Ak sa skener odtlačkov prstov nezobrazuje a skener je integrovaný do počítača, prejdite na webovú lokalitu výrobcu počítača.</span><span class="sxs-lookup"><span data-stu-id="d2086-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="d2086-126">V časti technickej podpory pre model vášho PC vyhľadajte ovládač pre Windows 10, ktorý môžete nainštalovať.</span><span class="sxs-lookup"><span data-stu-id="d2086-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="d2086-127">Ak je skener oddelený od PC (pripojeného cez USB), prejdite na webovú lokalitu výrobcu skenera a vyhľadajte a nainštalujte softvér ovládača zariadenia s Windowsom 10 pre model skenera, ktorý máte.</span><span class="sxs-lookup"><span data-stu-id="d2086-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
