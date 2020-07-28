---
title: Vyhľadanie stratených zariadení so systémom iOS pomocou intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440428"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="5922a-102">Vyhľadanie stratených zariadení so systémom iOS pomocou intune</span><span class="sxs-lookup"><span data-stu-id="5922a-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="5922a-103">Povolenie režimu strateného v zariadení so systémom iOS umožňuje správcovi zobraziť správu a telefónne číslo kontaktu na obrazovke uzamknutia.</span><span class="sxs-lookup"><span data-stu-id="5922a-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="5922a-104">Po povolení režimu strateného môže správca použiť akciu Vyhľadať zariadenie na identifikáciu fyzického umiestnenia zariadenia.</span><span class="sxs-lookup"><span data-stu-id="5922a-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="5922a-105">Akcia Vyhľadať zariadenie v programe Intune funguje so zariadeniami so systémom iOS a zobrazí umiestnenie konkrétneho zariadenia na mape.</span><span class="sxs-lookup"><span data-stu-id="5922a-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="5922a-106">Použitie tejto akcie vyžaduje, aby sa zariadenie so systémom iOS nachádzali v:</span><span class="sxs-lookup"><span data-stu-id="5922a-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="5922a-107">Režim pod dohľadom</span><span class="sxs-lookup"><span data-stu-id="5922a-107">Supervised mode</span></span>
- <span data-ttu-id="5922a-108">Režim straty</span><span class="sxs-lookup"><span data-stu-id="5922a-108">Lost mode</span></span>

<span data-ttu-id="5922a-109">Ďalšie informácie nájdete v téme [Povolenie strateného režimu v zariadeniach so systémom iOS/iPadOS so zariadeniami Intune](https://docs.microsoft.com/intune/device-lost-mode) a Vyhľadanie stratených alebo odcudzených [zariadení so systémom iOS/iPadOS so systémom Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="5922a-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="5922a-110">**Najčastejšie otázky**</span><span class="sxs-lookup"><span data-stu-id="5922a-110">**FAQ**</span></span>

<span data-ttu-id="5922a-111">Otázka: Vydal som vzdialenú akciu na odstránenie údajov spoločnosti zo zariadenia a teraz je uviaznutá v stave čakajúceho.</span><span class="sxs-lookup"><span data-stu-id="5922a-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="5922a-112">A: Ak chcete úspešne dokončiť vzdialenú akciu, cieľové zariadenie musí byť online a zdravé.</span><span class="sxs-lookup"><span data-stu-id="5922a-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="5922a-113">V nasledujúcich situáciách, vzdialená akcia zostane v stave čakania po dobu 30 dní, alebo kým zariadenie potvrdí príkaz:</span><span class="sxs-lookup"><span data-stu-id="5922a-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="5922a-114">Keï prístroj nemá konektivitu,</span><span class="sxs-lookup"><span data-stu-id="5922a-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="5922a-115">Keď zariadenie stratí stav správy pomocou intune</span><span class="sxs-lookup"><span data-stu-id="5922a-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="5922a-116">Ak si myslíte, že zariadenie už nie je v e-v zariadení v e-tom a nebude môcť odstrániť údaje spoločnosti, vyberte položku Odstrániť.</span><span class="sxs-lookup"><span data-stu-id="5922a-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="5922a-117">Odstránením sa odstráni záznam zariadenia tak, aby sa už nestraší v zozname zariadení Intune.</span><span class="sxs-lookup"><span data-stu-id="5922a-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="5922a-118">Ak sa zariadenie znova aktivuje, jeho používateľ ho bude musieť znova zaregistrovať.</span><span class="sxs-lookup"><span data-stu-id="5922a-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="5922a-119">Otázka: Prečo nie sú niektoré vzdialené akcie dostupné na používanie?</span><span class="sxs-lookup"><span data-stu-id="5922a-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="5922a-120">A: Nie všetky platformy podporujú všetky akcie vzdialeného zariadenia.</span><span class="sxs-lookup"><span data-stu-id="5922a-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="5922a-121">Nasledujúce vzdialené akcie sú špecifické pre platformu, takže sú k dispozícii len pre zaznamenané platformy.</span><span class="sxs-lookup"><span data-stu-id="5922a-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="5922a-122">Obísť zámok aktivácie (len pre iOS)</span><span class="sxs-lookup"><span data-stu-id="5922a-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="5922a-123">Nový začiatok (len v systéme Windows)</span><span class="sxs-lookup"><span data-stu-id="5922a-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="5922a-124">Režim straty (len pre iOS)</span><span class="sxs-lookup"><span data-stu-id="5922a-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="5922a-125">Vyhľadanie zariadenia (len pre iOS)</span><span class="sxs-lookup"><span data-stu-id="5922a-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="5922a-126">Reštartovať (len v systéme Windows)</span><span class="sxs-lookup"><span data-stu-id="5922a-126">Restart (Windows only)</span></span>

<span data-ttu-id="5922a-127">Ďalšie podrobnosti o jednotlivých akciách nájdete v téme [Akcie dostupného zariadenia](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="5922a-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>