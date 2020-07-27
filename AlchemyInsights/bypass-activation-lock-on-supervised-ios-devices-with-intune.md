---
title: Bypass activation lock on dohliadal iOS zariadenia s Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424213"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="47665-102">Bypass activation lock on dohliadal iOS zariadenia s Intune</span><span class="sxs-lookup"><span data-stu-id="47665-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="47665-103">Možnosť obísť zámok aktivácie v zariadeniach so systémom iOS uľahčuje obnovenie zo scenára, v ktorom používateľ povolí zámok aktivácie v podnikovom zariadení a potom opustí spoločnosť.</span><span class="sxs-lookup"><span data-stu-id="47665-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="47665-104">Predpoklady na obchádzanie zámku aktivácie zahŕňajú:</span><span class="sxs-lookup"><span data-stu-id="47665-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="47665-105">Zariadenie je, že je "pod dohľadom."</span><span class="sxs-lookup"><span data-stu-id="47665-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="47665-106">Zámok aktivácie je úspešne povolený pomocou politiky obmedzenia zariadenia systému iOS v intune.</span><span class="sxs-lookup"><span data-stu-id="47665-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="47665-107">Okrem toho, pri obchádzaní zámku aktivácie by ste mali:</span><span class="sxs-lookup"><span data-stu-id="47665-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="47665-108">Fyzicky majú zariadenie, ktoré je vymazané.</span><span class="sxs-lookup"><span data-stu-id="47665-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="47665-109">Skopírujte kód pred vydaním vymazanie.</span><span class="sxs-lookup"><span data-stu-id="47665-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="47665-110">**Upozornenie:** Utrite kód nie je malé a veľké písmená, takže "-" znaky nie sú povinné.</span><span class="sxs-lookup"><span data-stu-id="47665-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="47665-111">Podrobnosti nájdete v téme [Obídenie zámku aktivácie v zariadeniach so systémom iOS pod dohľadom s intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="47665-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="47665-112">**Najčastejšie otázky**</span><span class="sxs-lookup"><span data-stu-id="47665-112">**FAQ**</span></span>

<span data-ttu-id="47665-113">Otázka: **Vydal som vzdialenú akciu na odstránenie údajov spoločnosti zo zariadenia a teraz je uviaznutá v stave čakajúceho.**</span><span class="sxs-lookup"><span data-stu-id="47665-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="47665-114">A: Ak chcete úspešne dokončiť vzdialenú akciu, cieľové zariadenie musí byť online a zdravé.</span><span class="sxs-lookup"><span data-stu-id="47665-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="47665-115">V nasledujúcich situáciách, vzdialená akcia zostane v stave čakania po dobu 30 dní, alebo kým zariadenie potvrdí príkaz, keď zariadenie:</span><span class="sxs-lookup"><span data-stu-id="47665-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="47665-116">Nemá pripojenie.</span><span class="sxs-lookup"><span data-stu-id="47665-116">Does not have connectivity.</span></span>
- <span data-ttu-id="47665-117">Stratí stav správy s Intune.</span><span class="sxs-lookup"><span data-stu-id="47665-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="47665-118">Ak si myslíte, že zariadenie už nie je v e-v zariadení v e-tom a neodstráni údaje spoločnosti, vyberte položku Odstrániť.</span><span class="sxs-lookup"><span data-stu-id="47665-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="47665-119">Odstránením sa odstráni záznam zariadenia tak, aby sa už nestraší v zozname zariadení Intune.</span><span class="sxs-lookup"><span data-stu-id="47665-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="47665-120">Aby sa zariadenie znova opäť stalo aktívnym, jeho používateľ musí zariadenie znova zaregistrovať.</span><span class="sxs-lookup"><span data-stu-id="47665-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="47665-121">Otázka: **Prečo nie sú niektoré vzdialené akcie dostupné na používanie?**</span><span class="sxs-lookup"><span data-stu-id="47665-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="47665-122">A: Nie všetky platformy podporujú všetky akcie vzdialeného zariadenia.</span><span class="sxs-lookup"><span data-stu-id="47665-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="47665-123">Nasledujúce vzdialené akcie sú špecifické pre platformu.</span><span class="sxs-lookup"><span data-stu-id="47665-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="47665-124">Obísť zámok aktivácie (len pre iOS)</span><span class="sxs-lookup"><span data-stu-id="47665-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="47665-125">Nový začiatok (len v systéme Windows)</span><span class="sxs-lookup"><span data-stu-id="47665-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="47665-126">Režim straty (len pre iOS)</span><span class="sxs-lookup"><span data-stu-id="47665-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="47665-127">Vyhľadanie zariadenia (len pre iOS)</span><span class="sxs-lookup"><span data-stu-id="47665-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="47665-128">Reštartovať (len v systéme Windows)</span><span class="sxs-lookup"><span data-stu-id="47665-128">Restart (Windows only)</span></span>

<span data-ttu-id="47665-129">Ďalšie podrobnosti o jednotlivých akciách nájdete v téme [Akcie dostupného zariadenia](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="47665-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>