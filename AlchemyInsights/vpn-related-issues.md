---
title: Problémy súvisiace s VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555746"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="3fe37-102">Problémy súvisiace s VPN</span><span class="sxs-lookup"><span data-stu-id="3fe37-102">VPN related issues</span></span>

<span data-ttu-id="3fe37-103">Úspešná implementácia pripojenia VPN pre klientov MDM závisí od nasadený profil, ktorý správne odráža požiadavky infraštruktúry VPN.</span><span class="sxs-lookup"><span data-stu-id="3fe37-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="3fe37-104">Príslušné nastavenia pre klientske platformy, ktoré vyšetrujete, nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="3fe37-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="3fe37-105">Nastavenia holografického zariadenia vo Windowse 10 a Windowse na pridanie pripojení VPN pomocou aplikácie Intune</span><span class="sxs-lookup"><span data-stu-id="3fe37-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="3fe37-106">Pridanie nastavení VPN v zariadeniach so systémom iOS a iPadOS v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3fe37-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="3fe37-107">Nastavenia zariadenia android na konfiguráciu VPN v Intune</span><span class="sxs-lookup"><span data-stu-id="3fe37-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="3fe37-108">Pridanie nastavení VPN v zariadeniach so systémom macOS v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3fe37-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="3fe37-109">Ak váš vpn profil používa overovanie na základe certifikátu, uistite sa, že koreňový certifikát a klient overovanie certifikát profily prepojené s vpn profil sú úspešne nasadené.</span><span class="sxs-lookup"><span data-stu-id="3fe37-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="3fe37-110">**Bežné problémy**</span><span class="sxs-lookup"><span data-stu-id="3fe37-110">**Common Issues**</span></span>

<span data-ttu-id="3fe37-111">**Nasadil som vpn profil do zariadenia. Intune ukazuje, že to bolo úspešné, ale zariadenie nie je pripojenie k VPN.**</span><span class="sxs-lookup"><span data-stu-id="3fe37-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="3fe37-112">Úspešný stav znamená, že intune úspešne nasadil profil nakonfigurovaný.</span><span class="sxs-lookup"><span data-stu-id="3fe37-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="3fe37-113">Tieto konfigurácie sa však nemusia zhodovať s požiadavkami na sieť a alebo overenie.</span><span class="sxs-lookup"><span data-stu-id="3fe37-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="3fe37-114">Skontrolujte denníky v infraštruktúre a overovacia služba (na serveri VPN a NPS/Radius server) pre viac informácií o pokuse o pripojenie.</span><span class="sxs-lookup"><span data-stu-id="3fe37-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="3fe37-115">Na zhromažďovanie a kontrolu denníkov môže byť potrebné spolupracovať s tímom sieťovej infraštruktúry alebo s dodávateľom siete VPN tretej strany.</span><span class="sxs-lookup"><span data-stu-id="3fe37-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="3fe37-116">**Pri konfigurácii vlastnej siete VPN pre systém iOS nie je k dispozícii funkcia VPN pre vlastnú aplikáciu.**</span><span class="sxs-lookup"><span data-stu-id="3fe37-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="3fe37-117">Vpn pre zariadenia so systémom iOS v aplikácii Intune je momentálne k dispozícii pre konkrétny zoznam poskytovateľov a partnerov, ktorí musia pred konfiguráciou vpn pre jednotlivé aplikácie spĺňať aj požiadavky na certifikát.</span><span class="sxs-lookup"><span data-stu-id="3fe37-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="3fe37-118">Ďalšie informácie nájdete v téme [Nastavenie virtuálnej súkromnej siete (VPN) pre zariadenia so systémom iOS/iPadOS v programe Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="3fe37-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="3fe37-119">Ďalšie informácie o všetkých typoch pripojení VPN v programe Intune nájdete v téme [Vytvorenie profilov VPN na pripojenie k serverom VPN v programe Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="3fe37-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="3fe37-120">**iOS On-Demand VPN sa neštuduje pri prístupe k nakonfigurovanej doméne**</span><span class="sxs-lookup"><span data-stu-id="3fe37-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="3fe37-121">Ak chcete otestovať automatické nastavenie siete VPN, nastavte nasledujúce hodnoty:</span><span class="sxs-lookup"><span data-stu-id="3fe37-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="3fe37-122">Chcem urobiť nasledovné: Vyhodnoťte **každý pokus o pripojenie**</span><span class="sxs-lookup"><span data-stu-id="3fe37-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="3fe37-123">Vyberte, či sa chcete pripojiť: **V prípade potreby sa pripojte**</span><span class="sxs-lookup"><span data-stu-id="3fe37-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="3fe37-124">Keď používatelia pristupujú k týmto doménam: **názov** *cieľovej domény*</span><span class="sxs-lookup"><span data-stu-id="3fe37-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="3fe37-125">Ak vyššie uvedená konfigurácia nie je úspešná, pridajte nasledujúci prvok:</span><span class="sxs-lookup"><span data-stu-id="3fe37-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="3fe37-126">Ak je táto adresa URL nedosiahnuteľná, vynútiť pripojenie vpn: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="3fe37-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>