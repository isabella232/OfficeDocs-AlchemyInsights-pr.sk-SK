---
title: Riešenie problémov s existujúcim monitorom
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824594"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="098ff-102">Riešenie problémov s existujúcim monitorom</span><span class="sxs-lookup"><span data-stu-id="098ff-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="098ff-103">Na riešenie problémov s monitorom vyskúšajte tieto riešenia.</span><span class="sxs-lookup"><span data-stu-id="098ff-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="098ff-104">**Obnovenie obrazovky monitora:**</span><span class="sxs-lookup"><span data-stu-id="098ff-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="098ff-105">Stlačte naraz nasledujúce klávesy: kláves s logom Windows + Ctrl + Shift + B. Týmto sa obnoví komunikácia s ovládačom obrazovky.</span><span class="sxs-lookup"><span data-stu-id="098ff-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="098ff-106">Monitory budú na chvíľu blikať a po niekoľkých sekundách sa vrátia.</span><span class="sxs-lookup"><span data-stu-id="098ff-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="098ff-107">**Riešenie problémov s hardvérom monitora:**</span><span class="sxs-lookup"><span data-stu-id="098ff-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="098ff-108">Odpojte kábel, ktorý pripája PC k monitoru, a znova ho zapojte.</span><span class="sxs-lookup"><span data-stu-id="098ff-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="098ff-109">Odpojte od počítača akékoľvek iné ako základné zariadenia (napríklad adaptéry alebo doky).</span><span class="sxs-lookup"><span data-stu-id="098ff-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="098ff-110">**Ak ste si nedávno nainštalovali aktualizáciu do počítača, môžete vrátiť späť ovládač obrazovky:**</span><span class="sxs-lookup"><span data-stu-id="098ff-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="098ff-111">Vyberte **položku** Štart , zadajte **text Správca** zariadení a vo výsledkoch **vyberte** položku Správca zariadení.</span><span class="sxs-lookup"><span data-stu-id="098ff-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="098ff-112">Rozbaľte **časť Display adapters (Display adapters),** kliknite pravým tlačidlom myši na zobrazovací adaptér a vyberte položku **Vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="098ff-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="098ff-113">Prejdite na kartu **Ovládač** a vyberte položku **Vrátiť späť ovládač**.</span><span class="sxs-lookup"><span data-stu-id="098ff-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="098ff-114">Poznámka: Ak táto možnosť nie je k  dispozícii alebo je neaktívna, v nižšie uvedených možnostiach vyberte možnosť Nie a prejdite na ďalší krok.</span><span class="sxs-lookup"><span data-stu-id="098ff-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="098ff-115">Tieto zmeny sa prejavia až po reštartovaní počítača.</span><span class="sxs-lookup"><span data-stu-id="098ff-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="098ff-116">**Odinštalujte a znova nainštalujte ovládač obrazovky:**</span><span class="sxs-lookup"><span data-stu-id="098ff-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="098ff-117">Vyberte **položku** Štart , zadajte **text Správca** zariadení a vo výsledkoch **vyberte** položku Správca zariadení.</span><span class="sxs-lookup"><span data-stu-id="098ff-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="098ff-118">Rozbaľte **časť Display adapters (Zobrazovacie** adaptéry), kliknite pravým tlačidlom myši na svoj zobrazovací adaptér a vyberte možnosť **Uninstall device (Odinštalovať zariadenie).**</span><span class="sxs-lookup"><span data-stu-id="098ff-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="098ff-119">Začiarknite políčko vedľa položky **Odstrániť softvér ovládača pre toto zariadenie a vyberte** položku **Odinštalovať**.</span><span class="sxs-lookup"><span data-stu-id="098ff-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="098ff-120">Poznámka: V tejto fáze sa môže zobraziť výzva na reštartovanie počítača.</span><span class="sxs-lookup"><span data-stu-id="098ff-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="098ff-121">Pred reštartovaním si zapíšte zostávajúce pokyny.</span><span class="sxs-lookup"><span data-stu-id="098ff-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="098ff-122">Znova otvorte Správcu zariadení.</span><span class="sxs-lookup"><span data-stu-id="098ff-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="098ff-123">Rozbaľte **časť Display adapters (Zobrazovacie** adaptéry), kliknite pravým tlačidlom myši na zobrazovací adaptér a vyberte **položku Update Driver (Aktualizovať ovládač).**</span><span class="sxs-lookup"><span data-stu-id="098ff-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="098ff-124">Vyberte **položku Automaticky vyhľadávať softvér ovládača aktualizácie a** postupujte podľa pokynov na inštaláciu.</span><span class="sxs-lookup"><span data-stu-id="098ff-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>