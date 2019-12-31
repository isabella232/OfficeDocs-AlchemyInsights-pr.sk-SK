---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908724"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="8e980-102">Povolenie šifrovania BitLocker pomocou Intune</span><span class="sxs-lookup"><span data-stu-id="8e980-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="8e980-103">Intune Endpoint Protection politika môže byť použitá na konfigurovanie šifrovania BitLocker nastavenia pre zariadenia so systémom Windows.</span><span class="sxs-lookup"><span data-stu-id="8e980-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="8e980-104">Ďalšie informácie nájdete v téme [Windows 10 (a novšie) nastavenia na ochranu zariadení pomocou služby Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="8e980-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="8e980-105">Mali by ste si uvedomiť, že mnohé novšie zariadenia so systémom Windows 10 podporujú automatické šifrovanie BitLocker, ktoré sa spúšťa bez použitia politiky MDM.</span><span class="sxs-lookup"><span data-stu-id="8e980-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="8e980-106">To môže ovplyvniť uplatňovanie politiky, ak nie sú predvolené nastavenia nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="8e980-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="8e980-107">Ďalšie podrobnosti nájdete v nasledujúcich najčastejších otázkach.</span><span class="sxs-lookup"><span data-stu-id="8e980-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="8e980-108">Informácie o riešení problémov s šifrmi BitLocker nájdete [v téme Riešenie problémov s pravidlami šifrovania BitLocker v programe Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="8e980-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="8e980-109">**Najčastejšie otázky**</span><span class="sxs-lookup"><span data-stu-id="8e980-109">**FAQ**</span></span>

 <span data-ttu-id="8e980-110">Otázka: ktoré vydania systému Windows podporujú šifrovanie zariadenia pomocou politiky Endpoint Protection?</span><span class="sxs-lookup"><span data-stu-id="8e980-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="8e980-111">A: nastavenia v Intune Endpoint Protection politiky sú implementované pomocou [šifrovania BitLocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="8e980-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="8e980-112">Nie všetky vydania alebo zostavy systému Windows podporujú šifrovanie BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="8e980-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="8e980-113">V tomto okamihu sú podporované nasledujúce vydania systému Windows: Enterprise, Education, Mobile, Mobile Enterprise a Professional (build 1809 a novší).</span><span class="sxs-lookup"><span data-stu-id="8e980-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="8e980-114">Q: Ak zariadenie je už šifrované s BitLocker pomocou predvoleného nastavenia operačného systému pre metódu šifrovania a šifrovacia sila (XTS-AES-128), bude uplatňovať politiku s rôznymi nastaveniami automaticky spustí re-šifrovanie disku s novými nastaveniami?</span><span class="sxs-lookup"><span data-stu-id="8e980-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="8e980-115">A: nie.</span><span class="sxs-lookup"><span data-stu-id="8e980-115">A: No.</span></span> <span data-ttu-id="8e980-116">Ak chcete použiť nové šifrovacie nastavenia, jednotka musí byť najprv dešifrovaná.</span><span class="sxs-lookup"><span data-stu-id="8e980-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="8e980-117">**Poznámka:** Pre zariadenia, ktoré sa zaregistrujú s autopilot, automatické šifrovanie, ktoré by sa vyskytli počas OOBE sa nespúšťa, kým sa vyhodnotí politika Intune, čo umožňuje nastavenie založené na zásadách, ktoré sa použije namiesto predvolených hodnôt operačného systému.</span><span class="sxs-lookup"><span data-stu-id="8e980-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="8e980-118">Otázka: Ak je zariadenie šifrované v dôsledku uplatňovania politiky Intune, bude dešifrovať pri odstránení tejto politiky?</span><span class="sxs-lookup"><span data-stu-id="8e980-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="8e980-119">A: Odstránenie politiky súvisiace s šifrovaním nemá za následok dešifrovanie jednotiek, ktoré boli nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="8e980-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="8e980-120">Otázka: prečo Intune súlad politiky ukazujú, že moje zariadenie nemá BitLocker povolené, aj keď to je?</span><span class="sxs-lookup"><span data-stu-id="8e980-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="8e980-121">A: "BitLocker Enabled" nastavenie v Intune súladu politiky využíva Windows Device Health osvedčenie (DHA) klienta.</span><span class="sxs-lookup"><span data-stu-id="8e980-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="8e980-122">Tento klient len meria stav zariadenia v čase spúšťania.</span><span class="sxs-lookup"><span data-stu-id="8e980-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="8e980-123">Takže ak zariadenie nebolo reštartuje, pretože šifrovanie BitLocker bola dokončená, DHA klient služba nebude hlásiť BitLocker ako aktívny.</span><span class="sxs-lookup"><span data-stu-id="8e980-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 