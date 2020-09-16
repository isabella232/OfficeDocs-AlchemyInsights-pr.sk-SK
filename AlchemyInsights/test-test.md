---
title: Výrazy chýbajúce zo služby SharePoint Online term Store
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750466"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="bb6fb-102">Povolenie šifrovania BitLocker so službou Intune</span><span class="sxs-lookup"><span data-stu-id="bb6fb-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="bb6fb-103">Politika ochrany koncového bodu služby Intune sa môže použiť na konfigurovanie nastavení šifrovania Boitlocker pre zariadenia s Windowsom, ako je popísané v téme: windows10 (a novšie verzie) na ochranu zariadení pomocou služby Intune</span><span class="sxs-lookup"><span data-stu-id="bb6fb-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="bb6fb-104">Mali by ste vedieť, že mnohé novšie zariadenia s Windowsom 10 podporujú automatické šifrovanie šifrovania BitLocker, ktoré je spustené bez použitia politiky MDM.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="bb6fb-105">Môže to mať vplyv na uplatňovanie politiky, ak nie sú nakonfigurované iné ako predvolené nastavenia.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="bb6fb-106">Ďalšie podrobnosti nájdete v téme Najčastejšie otázky.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-106">See FAQ for more detail.</span></span>


<span data-ttu-id="bb6fb-107">FAQ   Q: ktoré vydania systému Windows podporujú šifrovanie zariadenia pomocou politiky koncového bodu ochrany?</span><span class="sxs-lookup"><span data-stu-id="bb6fb-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="bb6fb-108"> A: nastavenie politiky ochrany koncového bodu služby Intune sa implementuje pomocou funkcie BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="bb6fb-109">Nie všetky vydania ani zostavy Windowsu nepodporujú funkciu BitLocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="bb6fb-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="bb6fb-110">V tejto časovej verzii Windowsu: Enterprise; Podporované sú vzdelávacie, mobilné, mobilné podniky a profesionálna (od zostavy 1809).</span><span class="sxs-lookup"><span data-stu-id="bb6fb-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="bb6fb-111">Otázka: Ak je zariadenie už šifrované pomocou šifrovania BitLocker s použitím predvolených nastavení operačného systému pre metódu šifrovania a pevnosť šifrovania (XTS-AES-128), bude uplatňovať politiku s rôznymi nastaveniami automaticky spustiť opätovné šifrovanie jednotky s novým nastavením?</span><span class="sxs-lookup"><span data-stu-id="bb6fb-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="bb6fb-112">Odpoveď: Nie.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-112">A: No.</span></span> <span data-ttu-id="bb6fb-113">Ak chcete použiť nové nastavenia šifrovania, jednotka musí byť najprv dešifrovaná.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="bb6fb-114">Poznámka v prípade zariadení, ktoré sa zaregistrovali pomocou funkcie autopilot, automatické šifrovanie, ktoré sa vyskytne počas OOBE, sa nespustí, kým sa nevyhodnotí politika služby Intune, ktorá umožňuje použitie nastavení politiky na mieste predvolených hodnôt operačného systému.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="bb6fb-115">Otázka: Ak je zariadenie zašifrované ako dôsledok uplatňovania politiky služby Intune, po odstránení tejto politiky sa dešifruje?</span><span class="sxs-lookup"><span data-stu-id="bb6fb-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="bb6fb-116">A: Odstránenie politiky súvisiacej s šifrovaním nevedie k dešifrovaniu jednotiek, ktoré boli nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="bb6fb-117">Otázka: prečo politika v oblasti dodržiavania súladu so službou Intune zobrazuje, že moje zariadenie nemá zapnutú funkciu BitLocker, ale je to?</span><span class="sxs-lookup"><span data-stu-id="bb6fb-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="bb6fb-118">A: nastavenie šifrovania BitLocker v politike kompatibility služby Intune využíva klienta Windows Health Atestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="bb6fb-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="bb6fb-119">Tento klient meria stav zariadenia v čase spúšťania.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="bb6fb-120">Ak sa už po dokončení šifrovania šifrovania BitLocker nereštartuje zariadenie, klient služby DHA neohlási ako aktívnu funkciu BitLocker.</span><span class="sxs-lookup"><span data-stu-id="bb6fb-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>