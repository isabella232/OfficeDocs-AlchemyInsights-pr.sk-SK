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
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="10885-102">Použitie možnosti odomknúť odtlačok prsta vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="10885-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="10885-103">**Povoliť odtlačok prsta v systéme Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="10885-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="10885-104">Ak chcete Windows 10 odomknúť pomocou odtlačku prsta, musíte nastaviť odtlačok prsta Windows Hello pridaním (nechať Windows naučiť sa rozpoznávať) aspoň jedným prstom.</span><span class="sxs-lookup"><span data-stu-id="10885-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="10885-105">Prejdite do **časti nastavenia > kontá > možnosti prihlásenia** (alebo kliknite [sem](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="10885-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="10885-106">Dostupné možnosti prihlásenia budú uvedené.</span><span class="sxs-lookup"><span data-stu-id="10885-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="10885-107">Príklad:</span><span class="sxs-lookup"><span data-stu-id="10885-107">For example:</span></span>

    ![Možnosti prihlásenia.](media/sign-in-options.png)

2. <span data-ttu-id="10885-109">Kliknite alebo ťuknite na položku **odtlačok prsta v systéme Windows Hello**a potom kliknite na tlačidlo **nastaviť**.</span><span class="sxs-lookup"><span data-stu-id="10885-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="10885-110">V okne Nastavenie systému Windows Hello kliknite na položku **Začíname**.</span><span class="sxs-lookup"><span data-stu-id="10885-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="10885-111">Snímač odtlačkov prstov sa aktivuje a zobrazí sa výzva na zadanie prsta na senzore:</span><span class="sxs-lookup"><span data-stu-id="10885-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Snímač odtlačkov prstov.](media/fingerprint-sensor.png)

3. <span data-ttu-id="10885-113">Postupujte podľa pokynov, ktoré vás vyzve, aby ste opakovane skenovať prst.</span><span class="sxs-lookup"><span data-stu-id="10885-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="10885-114">Po dokončení tejto možnosti budete mať možnosť pridať ďalšie prsty, ktoré možno budete chcieť použiť na prihlasovanie.</span><span class="sxs-lookup"><span data-stu-id="10885-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="10885-115">Nabudúce sa prihlásite do systému Windows 10, budete mať možnosť pomocou odtlačku prsta tak urobiť.</span><span class="sxs-lookup"><span data-stu-id="10885-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="10885-116">**Odtlačok prsta v systéme Windows Hello nie je k dispozícii ako možnosť prihlásenia**</span><span class="sxs-lookup"><span data-stu-id="10885-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="10885-117">Ak sa odtlačok prsta v systéme Windows Hello nezobrazuje ako možnosť v **možnostiach prihlásenia**, znamená to, že systém Windows nevie o žiadnej čítačke/skeneri odtlačkov prstov pripojenom k počítaču alebo že systémová politika zabraňuje jej používaniu (Ak napríklad počítač spravuje vaše pracovisko).</span><span class="sxs-lookup"><span data-stu-id="10885-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="10885-118">Riešenie problémov s:</span><span class="sxs-lookup"><span data-stu-id="10885-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="10885-119">Na paneli úloh vyberte tlačidlo **Štart** a vyhľadajte položku **Správca zariadení**.</span><span class="sxs-lookup"><span data-stu-id="10885-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="10885-120">Kliknutím alebo ťuknutím otvorte **správcu zariadení**.</span><span class="sxs-lookup"><span data-stu-id="10885-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="10885-121">V Správcovi zariadení rozbaľte položku Biometrické zariadenia kliknutím na jeho Chevron.</span><span class="sxs-lookup"><span data-stu-id="10885-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrických zariadení.](media/biometric-devices.png)

4. <span data-ttu-id="10885-123">Snímač odtlačkov prstov by mal byť uvedený ako biometrické zariadenie, ako je napríklad skener Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="10885-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrických zariadení.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="10885-125">Ak sa skener odtlačkov prstov nezobrazuje a skener je integrovaný do počítača, prejdite na webovú lokalitu výrobcu počítača.</span><span class="sxs-lookup"><span data-stu-id="10885-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="10885-126">V časti Technická podpora pre model počítača vyhľadajte ovládač pre systém Windows 10 pre skener, ktorý môžete nainštalovať.</span><span class="sxs-lookup"><span data-stu-id="10885-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="10885-127">Ak je skener oddelený od počítača (pripojeného cez USB), prejdite na webovú lokalitu výrobcu skenera a vyhľadajte a nainštalujte softvér ovládača zariadenia Windows 10 pre model skenera, ktorý máte.</span><span class="sxs-lookup"><span data-stu-id="10885-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
