---
title: Chýbajúce podmienky v ukladacom priestore SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766868"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="fe307-102">Povolenie šifrovania BitLocker pomocou Intune</span><span class="sxs-lookup"><span data-stu-id="fe307-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="fe307-103">Intune Endpoint Protection politiky môžu byť použité na konfigurovanie Boitlocker nastavenia šifrovania pre zariadenia so systémom Windows, ako je opísané v: windows10 (a novšie) nastavenia na ochranu zariadení pomocou Intune</span><span class="sxs-lookup"><span data-stu-id="fe307-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="fe307-104">Mali by ste si uvedomiť, že mnohé novšie zariadenia so systémom Windows 10 podporujú automatické šifrovanie BitLocker, ktoré sa spúšťa bez použitia politiky MDM.</span><span class="sxs-lookup"><span data-stu-id="fe307-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="fe307-105">To môže ovplyvniť uplatňovanie politiky, ak nie sú nakonfigurované predvolené nastavenia.</span><span class="sxs-lookup"><span data-stu-id="fe307-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="fe307-106">Ďalšie podrobnosti nájdete v téme Najčastejšie otázky.</span><span class="sxs-lookup"><span data-stu-id="fe307-106">See FAQ for more detail.</span></span>


<span data-ttu-id="fe307-107">FAQ  Q: ktoré vydania systému Windows podporuje šifrovanie zariadenia pomocou Endpoint Protection Policy?</span><span class="sxs-lookup"><span data-stu-id="fe307-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="fe307-108"> A: nastavenia v Intune Endpoint Protection politiky sú implementované pomocou šifrovania BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="fe307-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="fe307-109">Nie všetky vydania ani zostavy systému Windows podporujú šifrovanie BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="fe307-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="fe307-110">V tomto okamihu vydania systému Windows: Enterprise; Vzdelávanie, mobilné, mobilné podnikanie a profesionálne (od Build 1809 ďalej) sú podporované.</span><span class="sxs-lookup"><span data-stu-id="fe307-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="fe307-111">Q: Ak zariadenie je už šifrované s BitLocker pomocou predvoleného nastavenia operačného systému pre metódu šifrovania a šifrovacia sila (XTS-AES-128) bude uplatňovať politiku s rôznymi nastaveniami automaticky spustí re-šifrovanie disku s novými nastaveniami?</span><span class="sxs-lookup"><span data-stu-id="fe307-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="fe307-112">A: nie.</span><span class="sxs-lookup"><span data-stu-id="fe307-112">A: No.</span></span> <span data-ttu-id="fe307-113">Ak chcete použiť nové nastavenie šifrovania, jednotka musí byť najprv dešifrovaná.</span><span class="sxs-lookup"><span data-stu-id="fe307-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="fe307-114">Poznámka: pre zariadenia, ktoré sa zaregistrujú s autopilot automatické šifrovanie, ktoré by sa vyskytli počas OOBE nie je spustená, kým sa vyhodnotí politika Intune, ktorá umožňuje politiky založené nastavenia použiť namiesto predvolené OS</span><span class="sxs-lookup"><span data-stu-id="fe307-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="fe307-115">Q Ak je zariadenie šifrované v dôsledku uplatňovania politiky Intune bude dešifrovať pri odstránení tejto politiky?</span><span class="sxs-lookup"><span data-stu-id="fe307-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="fe307-116">A: odstránenie šifrovania súvisiace politiky nemá za následok dešifrovanie jednotiek, ktoré boli nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="fe307-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="fe307-117">Otázka: prečo Intune súlad politiky ukazujú, že moje zariadenie nemá "BitLocker Enabled", ale to je?</span><span class="sxs-lookup"><span data-stu-id="fe307-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="fe307-118">A: "BitLocker Enabled" nastavenie v Intune súladu politiky využíva Windows Device Health osvedčenie (DHA) klienta.</span><span class="sxs-lookup"><span data-stu-id="fe307-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="fe307-119">Tento klient len meria stav zariadenia v čase spúšťania.</span><span class="sxs-lookup"><span data-stu-id="fe307-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="fe307-120">Takže ak zariadenie nebolo reštartuje, pretože šifrovanie BitLocker bola dokončená služba DHA klient nebude hlásiť BitLocker ako aktívny.</span><span class="sxs-lookup"><span data-stu-id="fe307-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>