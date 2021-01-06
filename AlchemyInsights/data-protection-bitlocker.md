---
title: DataProtection – BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768832"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="ba89c-102">Povolenie šifrovania BitLocker so službou Intune</span><span class="sxs-lookup"><span data-stu-id="ba89c-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="ba89c-103">Politika ochrany koncového bodu služby Intune sa môže použiť na konfiguráciu nastavení šifrovania šifrovania BitLocker pre zariadenia s Windowsom.</span><span class="sxs-lookup"><span data-stu-id="ba89c-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="ba89c-104">Ďalšie informácie nájdete v téme [nastavenia Windowsu 10 (a novšie) na ochranu zariadení pomocou služby Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="ba89c-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="ba89c-105">Mali by ste vedieť, že mnoho novších zariadení s Windowsom 10 podporuje automatické šifrovanie BitLocker, ktoré je spustené bez použitia politiky MDM.</span><span class="sxs-lookup"><span data-stu-id="ba89c-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="ba89c-106">Môže to mať vplyv na uplatňovanie politiky v prípade, že nie sú nakonfigurované predvolené nastavenia.</span><span class="sxs-lookup"><span data-stu-id="ba89c-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="ba89c-107">Ďalšie podrobnosti nájdete v týchto FAQ.</span><span class="sxs-lookup"><span data-stu-id="ba89c-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="ba89c-108">Ďalšie informácie o riešení problémov so šifrovaním BitLocker nájdete [v téme Riešenie problémov s politikami šifrovania BitLocker v službe Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="ba89c-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="ba89c-109">**Najčastejšie otázky**</span><span class="sxs-lookup"><span data-stu-id="ba89c-109">**FAQ**</span></span>

<span data-ttu-id="ba89c-110">Otázka: ktoré vydania systému Windows podporujú šifrovanie zariadenia pomocou politiky koncového bodu ochrany?</span><span class="sxs-lookup"><span data-stu-id="ba89c-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="ba89c-111">A: nastavenie politiky ochrany koncového bodu služby Intune sa implementuje pomocou [funkcie BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="ba89c-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="ba89c-112">Nie všetky vydania ani zostavy Windowsu podporujú funkciu BitLocker CSP.</span><span class="sxs-lookup"><span data-stu-id="ba89c-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="ba89c-113">Otázka: ako môže byť funkcia BitLocker povolená v zariadeniach bez nutnosti interakcie koncového používateľa?</span><span class="sxs-lookup"><span data-stu-id="ba89c-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="ba89c-114">A: kým sa splnia potrebné predpoklady, je možné povoliť šifrovanie BitLocker tiché šifrovanie prostredníctvom služby Intune.</span><span class="sxs-lookup"><span data-stu-id="ba89c-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="ba89c-115">Pozrite si Podrobnosti o požiadavkách na zariadenie a príklade nastavenie politiky na zapnutie tichého šifrovania v nasledujúcom dokumente: [tiché povolenie šifrovania BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="ba89c-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="ba89c-116">Otázka: Ak je zariadenie už šifrované pomocou šifrovania BitLocker s použitím predvolených nastavení operačného systému pre metódu šifrovania a pevnosť šifrovania (XTS-AES-128), bude uplatňovať politiku s rôznymi nastaveniami automaticky spustiť opätovné šifrovanie jednotky s novými nastaveniami?</span><span class="sxs-lookup"><span data-stu-id="ba89c-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="ba89c-117">Odpoveď: Nie.</span><span class="sxs-lookup"><span data-stu-id="ba89c-117">A: No.</span></span> <span data-ttu-id="ba89c-118">Ak chcete použiť nové nastavenie šifrovania, jednotka musí byť najprv dešifrovaná.</span><span class="sxs-lookup"><span data-stu-id="ba89c-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="ba89c-119">**Poznámka:** V prípade zariadení, ktoré sa zaregistrovali pomocou funkcie autopilot, sa automatické šifrovanie, ktoré sa vyskytne počas OOBE, nespustí, kým sa vyhodnotí politika služby Intune, ktorá umožňuje použiť nastavenia na základe politiky namiesto predvolených hodnôt operačného systému.</span><span class="sxs-lookup"><span data-stu-id="ba89c-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="ba89c-120">Otázka: Ak je zariadenie zašifrované ako dôsledok uplatňovania politiky služby Intune, bude sa dešifrovať pri odstránení tejto politiky?</span><span class="sxs-lookup"><span data-stu-id="ba89c-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="ba89c-121">A: Odstránenie politiky súvisiacej s šifrovaním nespôsobí dešifrovanie jednotiek, ktoré boli nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="ba89c-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="ba89c-122">Otázka: prečo sa v politike zabezpečenia služby Intune zobrazuje, že moje zariadenie nemá zapnutú funkciu BitLocker, dokonca aj napriek tomu, že je?</span><span class="sxs-lookup"><span data-stu-id="ba89c-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="ba89c-123">A: nastavenie šifrovania BitLocker v politike zabezpečenia dodržiavania služby Intune využíva klienta Windows Health Atestation (DHA).</span><span class="sxs-lookup"><span data-stu-id="ba89c-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="ba89c-124">Tento klient meria stav zariadenia v čase spúšťania.</span><span class="sxs-lookup"><span data-stu-id="ba89c-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="ba89c-125">Ak sa však zariadenie po dokončení šifrovania šifrovania BitLocker nereštartovalo, Služba pre klientov DHA neohlási ako aktívnu funkciu BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ba89c-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 