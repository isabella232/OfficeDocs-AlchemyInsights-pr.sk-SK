---
title: Riešenie problémov s nasadením certifikátu overenia klienta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555810"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="b3b74-102">Riešenie problémov s nasadením certifikátu overenia klienta</span><span class="sxs-lookup"><span data-stu-id="b3b74-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="b3b74-103">Intune NDES/SCEP a PKCS/PFX klientske certifikáty profily sa bežne používajú v spojení s inými typmi profilov, ako je Wifi, VPN a e-mail, aby používatelia mohli overiť podnikové zdroje.</span><span class="sxs-lookup"><span data-stu-id="b3b74-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="b3b74-104">Keď tieto typy profilov sú prepojené s profilom certifikátu klienta sú závislé na úspešné nasadenie tohto profilu.</span><span class="sxs-lookup"><span data-stu-id="b3b74-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="b3b74-105">Počiatočné nastavenie infraštruktúry a súvisiace konfigurácie profilu certifikátu klienta často vyžadujú riešenie problémov.</span><span class="sxs-lookup"><span data-stu-id="b3b74-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="b3b74-106">Podrobný sprievodca úspešné nastavenie konektora NDES a pokyny na riešenie problémov na izoláciu problémov s nasadením certifikátu nájdete na:</span><span class="sxs-lookup"><span data-stu-id="b3b74-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="b3b74-107">Konfigurácia infraštruktúry na podporu protokolu SCEP s intune</span><span class="sxs-lookup"><span data-stu-id="b3b74-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="b3b74-108">Prehľad problémov s profilmi certifikátov SCEP s Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b3b74-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="b3b74-109">Na overenie konfigurácie použite odkazované skripty prostredia PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b3b74-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="b3b74-110">Ďalšie informácie nájdete v téme [Skripty na overenie konektora certifikátu intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="b3b74-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="b3b74-111">**Ďalšie bežné otázky**</span><span class="sxs-lookup"><span data-stu-id="b3b74-111">**Other common issues**</span></span>

<span data-ttu-id="b3b74-112">**Pri pokuse o inštaláciu konektora certifikátu Intune na konektor NDES server, dostanem správu, "heslo v žiadosti o certifikát nie je možné overiť. To môže byť použitý už. Získať nové heslo na odoslanie s touto požiadavkou."**</span><span class="sxs-lookup"><span data-stu-id="b3b74-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="b3b74-113">Toto hlásenie znamená, že musíte spustiť inštaláciu konektora certifikátu ako správca.</span><span class="sxs-lookup"><span data-stu-id="b3b74-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="b3b74-114">V niektorých prostrediach servery, kde je spustený certifikát Intune, musia na pripojenie k intune použiť server proxy, a preto musí certifikačná konzola používať server proxy.</span><span class="sxs-lookup"><span data-stu-id="b3b74-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="b3b74-115">V niektorých prípadoch NDES konektor ignoruje nakonfigurovaný nastavenia servera proxy a môže byť potrebné nakonfigurovať nastavenia servera proxy pri spustení v kontexte zabezpečenia LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="b3b74-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="b3b74-116">Riešením je spustiť program Internet Explorer ako systém a nakonfigurovať proxy v IE.</span><span class="sxs-lookup"><span data-stu-id="b3b74-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="b3b74-117">Po reštarte služby Konektor Intune, Konektor NDES sa pripojí k Intune.</span><span class="sxs-lookup"><span data-stu-id="b3b74-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="b3b74-118">**Používateľské zariadenia už nedostávajú certifikáty SCEP z NDES.**</span><span class="sxs-lookup"><span data-stu-id="b3b74-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="b3b74-119">Je možné, že certifikát overenia klienta vydaný na server NDES a zadaný počas inštalácie konektora NDES uplynula alebo chýba.</span><span class="sxs-lookup"><span data-stu-id="b3b74-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="b3b74-120">Riešenie:</span><span class="sxs-lookup"><span data-stu-id="b3b74-120">To resolve:</span></span> 
 
1. <span data-ttu-id="b3b74-121">Odinštalovať konektor NDES.</span><span class="sxs-lookup"><span data-stu-id="b3b74-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="b3b74-122">Tieto podrobnosti použite na vyžiadanie nového certifikátu overenia klienta alebo servera:</span><span class="sxs-lookup"><span data-stu-id="b3b74-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="b3b74-123">Názov predmetu: CN = externý fqdn</span><span class="sxs-lookup"><span data-stu-id="b3b74-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="b3b74-124">Alternatívny názov predmetu (obe sú povinné): DNS = externé fqdn, DNS = interné fqdn</span><span class="sxs-lookup"><span data-stu-id="b3b74-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="b3b74-125">Preinštalujte konektor NDES s novým certifikátom.</span><span class="sxs-lookup"><span data-stu-id="b3b74-125">Reinstall the NDES connector with the new certificate.</span></span>