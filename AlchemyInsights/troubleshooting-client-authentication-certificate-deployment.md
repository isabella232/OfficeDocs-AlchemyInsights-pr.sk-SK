---
title: Riešenie problémov s nasadením certifikátu overenia klienta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659001"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="55472-102">Riešenie problémov s nasadením certifikátu overenia klienta</span><span class="sxs-lookup"><span data-stu-id="55472-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="55472-103">Profily klientskych certifikátov služby Intune NDES/SCEP a PKCS/PFX sa bežne používajú v spojení s inými typmi profilov, ako je napríklad WiFi, VPN a e-mailom, aby mohli používatelia autentifikovať podnikové zdroje.</span><span class="sxs-lookup"><span data-stu-id="55472-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="55472-104">Keď sú tieto typy profilu prepojené s profilom certifikátu klienta, závisia od úspešného nasadenia daného profilu.</span><span class="sxs-lookup"><span data-stu-id="55472-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="55472-105">Nastavenie počiatočnej infraštruktúry a súvisiaca Konfigurácia profilu certifikátu klienta často vyžadujú riešenie problémov.</span><span class="sxs-lookup"><span data-stu-id="55472-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="55472-106">Podrobný návod na úspešné Nastavenie konektora NDES a pokyny na riešenie problémov na izolovanie problémov s nasadením certifikátu nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="55472-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="55472-107">Konfigurácia infraštruktúry na podporu protokolu SCEP so službou Intune</span><span class="sxs-lookup"><span data-stu-id="55472-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="55472-108">Prehľad na riešenie problémov s profilmi certifikátu protokolu SCEP so službou Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="55472-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="55472-109">Na overenie konfigurácie použite odkazové skripty prostredia PowerShell.</span><span class="sxs-lookup"><span data-stu-id="55472-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="55472-110">Ďalšie informácie nájdete v téme [skripty na overenie konektora služby Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="55472-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="55472-111">**Ďalšie bežné problémy**</span><span class="sxs-lookup"><span data-stu-id="55472-111">**Other common issues**</span></span>

<span data-ttu-id="55472-112">**Pri pokuse o inštaláciu konektora certifikátu Intune na serveri konektora NDES sa zobrazí hlásenie "heslo v žiadosti o certifikát nie je možné overiť. Môže sa použiť už. Získajte nové heslo na odoslanie s touto požiadavkou.**</span><span class="sxs-lookup"><span data-stu-id="55472-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="55472-113">Toto hlásenie znamená, že je potrebné spustiť inštaláciu konektora certifikátu ako správca.</span><span class="sxs-lookup"><span data-stu-id="55472-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="55472-114">V niektorých prostrediach musia servery, v ktorých sa spustí certifikát služby Intune, použiť server proxy na pripojenie k službe Intune, a preto musí konektor certifikátu použiť server proxy.</span><span class="sxs-lookup"><span data-stu-id="55472-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="55472-115">V niektorých prípadoch NDES spojnica ignoruje nakonfigurované nastavenia servera proxy a pri spustení v kontexte zabezpečenia funkcie LocalSystem môže byť potrebné nakonfigurovať nastavenia servera proxy.</span><span class="sxs-lookup"><span data-stu-id="55472-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="55472-116">Riešením je spustiť Internet Explorer ako systém a nakonfigurovať server proxy v programe IE.</span><span class="sxs-lookup"><span data-stu-id="55472-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="55472-117">Po reštartovaní služby Intune Connector sa konektor NDES pripojí k službe Intune.</span><span class="sxs-lookup"><span data-stu-id="55472-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="55472-118">**Používateľské zariadenia už neprijímajú certifikáty SCEP z NDES.**</span><span class="sxs-lookup"><span data-stu-id="55472-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="55472-119">Je možné, že certifikát klientskeho overenia vydaný na server NDES a zadaný počas inštalácie konektora NDES uplynul alebo chýba.</span><span class="sxs-lookup"><span data-stu-id="55472-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="55472-120">Ak chcete vyriešiť:</span><span class="sxs-lookup"><span data-stu-id="55472-120">To resolve:</span></span> 
 
1. <span data-ttu-id="55472-121">Odinštalujte konektor NDES.</span><span class="sxs-lookup"><span data-stu-id="55472-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="55472-122">Pomocou týchto podrobností si môžete vyžiadať nový certifikát overenia klienta alebo overenie servera:</span><span class="sxs-lookup"><span data-stu-id="55472-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="55472-123">Názov predmetu: CN = external FQDN</span><span class="sxs-lookup"><span data-stu-id="55472-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="55472-124">Alternatívny názov predmetu (vyžaduje sa oboje): DNS = externý FQDN, DNS = Internal FQDN</span><span class="sxs-lookup"><span data-stu-id="55472-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="55472-125">Preinštalujte konektor NDES s novým certifikátom.</span><span class="sxs-lookup"><span data-stu-id="55472-125">Reinstall the NDES connector with the new certificate.</span></span>