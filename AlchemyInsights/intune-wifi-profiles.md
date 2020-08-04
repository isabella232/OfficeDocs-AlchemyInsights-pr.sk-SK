---
title: Profily Wi-Fi intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555813"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="49fb9-102">Profily Wi-Fi intune</span><span class="sxs-lookup"><span data-stu-id="49fb9-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="49fb9-103">Úspešná implementácia Wi-Fi pripojenia pre KLIENTOV MDM závisí od správne nasadený profil, ktorý odráža požiadavky podnikovej Wi-Fi infraštruktúry.</span><span class="sxs-lookup"><span data-stu-id="49fb9-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="49fb9-104">Ak chcete skontrolovať príslušné nastavenia pre klientske platformy, ktoré vyšetrujete, nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="49fb9-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="49fb9-105">Pridanie nastavení Wi-Fi pre zariadenia so systémom Android v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="49fb9-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="49fb9-106">Pridanie nastavení Wi-Fi pre zariadenia určené pre Android Enterprise a plne spravované zariadenia v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="49fb9-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="49fb9-107">Pridanie nastavení Wi-Fi pre zariadenia so systémom iOS a iPadOS v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="49fb9-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="49fb9-108">Pridanie nastavení Wi-Fi pre Windows 10 a novšie zariadenia v službe Intune</span><span class="sxs-lookup"><span data-stu-id="49fb9-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="49fb9-109">Import nastavení Wi-Fi pre zariadenia so systémom Windows v programe Intune</span><span class="sxs-lookup"><span data-stu-id="49fb9-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="49fb9-110">**Bežné problémy**</span><span class="sxs-lookup"><span data-stu-id="49fb9-110">**Common Issues**</span></span>

<span data-ttu-id="49fb9-111">**Nasadzujem profil Wi-Fi, ktorý je závislý od nasadeného certifikátu zadaného v profile Wi-Fi. Konfiguračné profily však zobrazujú stav chyby.**</span><span class="sxs-lookup"><span data-stu-id="49fb9-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="49fb9-112">Skontrolujte, či vaše zariadenie prijalo certifikát.</span><span class="sxs-lookup"><span data-stu-id="49fb9-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="49fb9-113">V časti Intune prejdite **na položku Všetky** zariadenia a vyberte > **zariadenia**.</span><span class="sxs-lookup"><span data-stu-id="49fb9-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="49fb9-114">Skontrolujte, či všetky očakávané profily sú uvedené a v úspešnom stave.</span><span class="sxs-lookup"><span data-stu-id="49fb9-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="49fb9-115">Ak máte v reťazci certifikátov dočasné certifikáty, v prípade profilu Android sa uistite, že sú nasadené do zariadení s Androidom.</span><span class="sxs-lookup"><span data-stu-id="49fb9-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="49fb9-116">Ak chcete skontrolovať stav certifikátu, prejdite na **Profily konfigurácie**  >  **zariadenia**  >  **Android stredne CA Vlastnosti**  >  **dôveryhodný**  >  **certifikát**.</span><span class="sxs-lookup"><span data-stu-id="49fb9-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="49fb9-117">Ak sa chyby naďalej vyskytujú, prečítajte si postupy a časti na riešenie problémov.</span><span class="sxs-lookup"><span data-stu-id="49fb9-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="49fb9-118">Ďalšie informácie nájdete v téme Prehľad [riešenia problémov s profilmi certifikátov SCEP s Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="49fb9-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="49fb9-119">**Nasadel som profil Wi-Fi do zariadenia. Intune ukazuje, že to bolo úspešné, ale zariadenie nie je pripojenie k Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="49fb9-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="49fb9-120">Úspešný stav znamená, že intune úspešne nasadil profil nakonfigurovaný.</span><span class="sxs-lookup"><span data-stu-id="49fb9-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="49fb9-121">Tieto konfigurácie sa však nemusia zhodovať s požiadavkami na sieť a alebo overenie.</span><span class="sxs-lookup"><span data-stu-id="49fb9-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="49fb9-122">Ďalšie podrobnosti o pokuse o pripojenie, skontrolujte denníky v infraštruktúre a overovacia služba (na radiči bodu Prístupu Wi-Fi a NPS/Radius server).</span><span class="sxs-lookup"><span data-stu-id="49fb9-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="49fb9-123">Na zhromažďovanie a kontrolu denníkov môže byť potrebné spolupracovať s tímom sieťovej infraštruktúry alebo s dodávateľom Wi-Fi tretej strany.</span><span class="sxs-lookup"><span data-stu-id="49fb9-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>