---
title: Riešenie problémov s existujúcim monitorom
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690726"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="7dc04-102">Riešenie problémov s existujúcim monitorom</span><span class="sxs-lookup"><span data-stu-id="7dc04-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="7dc04-103">Vyskúšajte tieto riešenia na riešenie problémov s monitorom.</span><span class="sxs-lookup"><span data-stu-id="7dc04-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="7dc04-104">**Obnovenie zobrazenia monitora:**</span><span class="sxs-lookup"><span data-stu-id="7dc04-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="7dc04-105">Súčasne stláčajte nasledujúce klávesy: kláves s logom Windows + CTRL + SHIFT + B. Týmto sa obnoví komunikácia s ovládačom grafickej karty.</span><span class="sxs-lookup"><span data-stu-id="7dc04-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="7dc04-106">Monitory budú na chvíľu blikať a po niekoľkých sekundách sa vrátia späť.</span><span class="sxs-lookup"><span data-stu-id="7dc04-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="7dc04-107">**Riešenie problémov s hardvérom monitora:**</span><span class="sxs-lookup"><span data-stu-id="7dc04-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="7dc04-108">Odpojte kábel spájajúci PC s monitorom a znova ho zapojte.</span><span class="sxs-lookup"><span data-stu-id="7dc04-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="7dc04-109">Odpojte všetky nepodstatné zariadenia z počítača (napríklad adaptéry alebo doky).</span><span class="sxs-lookup"><span data-stu-id="7dc04-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="7dc04-110">**Ak ste nedávno nainštalovali aktualizáciu do počítača, môžete vrátiť späť svoj ovládač zobrazenia:**</span><span class="sxs-lookup"><span data-stu-id="7dc04-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="7dc04-111">Vyberte položku **Štart**, zadajte výraz **Správca zariadení**a z výsledkov vyberte položku **Správca zariadení** .</span><span class="sxs-lookup"><span data-stu-id="7dc04-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="7dc04-112">Rozbaľte časť **zobrazovacie adaptéry** , kliknite pravým tlačidlom myši na zobrazovací adaptér, ANDS vyberte položku **Vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="7dc04-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="7dc04-113">Prejdite na kartu **ovládač** a vyberte položku vrátiť **ovládač**.</span><span class="sxs-lookup"><span data-stu-id="7dc04-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="7dc04-114">Poznámka: Ak táto možnosť nie je k dispozícii alebo je neaktívna, vyberte položku **nie** z nižšie uvedenej možnosti, čím prejdete na ďalší krok.</span><span class="sxs-lookup"><span data-stu-id="7dc04-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="7dc04-115">Možno bude potrebné reštartovať počítač, aby sa tieto zmeny prejavili.</span><span class="sxs-lookup"><span data-stu-id="7dc04-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="7dc04-116">**Odinštalovanie a opätovné nainštalovanie ovládača zobrazenia:**</span><span class="sxs-lookup"><span data-stu-id="7dc04-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="7dc04-117">Vyberte položku **Štart**, zadajte výraz **Správca zariadení**a z výsledkov vyberte položku **Správca zariadení** .</span><span class="sxs-lookup"><span data-stu-id="7dc04-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="7dc04-118">Rozbaľte časť **zobrazovacie adaptéry** , kliknite pravým tlačidlom myši na zobrazovací adaptér, ANDS vyberte položku **odinštalovať zariadenie**.</span><span class="sxs-lookup"><span data-stu-id="7dc04-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="7dc04-119">Začiarknite políčko vedľa položky **odstrániť softvér ovládača pre toto zariadenie** a vyberte položku **odinštalovať**.</span><span class="sxs-lookup"><span data-stu-id="7dc04-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="7dc04-120">Poznámka: môže sa zobraziť výzva na reštartovanie počítača v tejto fáze.</span><span class="sxs-lookup"><span data-stu-id="7dc04-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="7dc04-121">Pred reštartovaním nezabudnite napísať zvyšné pokyny.</span><span class="sxs-lookup"><span data-stu-id="7dc04-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="7dc04-122">Znova otvorte správcu zariadení.</span><span class="sxs-lookup"><span data-stu-id="7dc04-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="7dc04-123">Rozbaľte časť **zobrazovacie adaptéry** , kliknite pravým tlačidlom myši na zobrazovací adaptér a vyberte položku **aktualizovať ovládač**.</span><span class="sxs-lookup"><span data-stu-id="7dc04-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="7dc04-124">Vyberte položku **automaticky vyhľadávať na aktualizáciu softvéru ovládača** a postupujte podľa pokynov na inštaláciu.</span><span class="sxs-lookup"><span data-stu-id="7dc04-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>