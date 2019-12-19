---
title: Riešenie problémov s existujúcim monitorom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738583"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="82f40-102">Riešenie problémov s existujúcim monitorom</span><span class="sxs-lookup"><span data-stu-id="82f40-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="82f40-103">Vyskúšajte tieto riešenia na riešenie problémov s monitorom.</span><span class="sxs-lookup"><span data-stu-id="82f40-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="82f40-104">**Obnovte obrazovku monitora:**</span><span class="sxs-lookup"><span data-stu-id="82f40-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="82f40-105">Súčasne stlačte nasledujúce klávesy: klávesa Windows + CTRL + SHIFT + B. Tým sa obnoví komunikácia s ovládačom grafickej karty.</span><span class="sxs-lookup"><span data-stu-id="82f40-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="82f40-106">Vaše monitory budú blikať na okamih a vrátiť sa po niekoľkých sekundách.</span><span class="sxs-lookup"><span data-stu-id="82f40-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="82f40-107">**Riešenie problémov s hardvérom monitora:**</span><span class="sxs-lookup"><span data-stu-id="82f40-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="82f40-108">Odpojte kábel pripájajúci počítač k monitoru a znova ho zapojte.</span><span class="sxs-lookup"><span data-stu-id="82f40-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="82f40-109">Odpojte od počítača všetky nepodstatné zariadenia (napríklad adaptéry alebo doky).</span><span class="sxs-lookup"><span data-stu-id="82f40-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="82f40-110">**Ak ste nedávno nainštalovali aktualizáciu v počítači, môžete vrátiť ovládač obrazovky:**</span><span class="sxs-lookup"><span data-stu-id="82f40-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="82f40-111">Vyberte položku **Štart**, zadajte **Správca zariadení**a z výsledkov vyberte položku **Správca zariadení** .</span><span class="sxs-lookup"><span data-stu-id="82f40-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="82f40-112">Rozbaľte sekciu **zobrazovacie adaptéry** , kliknite pravým tlačidlom myši na zobrazovací adaptér, ANDS vyberte **Vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="82f40-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="82f40-113">Prejdite na kartu **ovládač** a vyberte položku vrátiť **ovládač**.</span><span class="sxs-lookup"><span data-stu-id="82f40-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="82f40-114">Poznámka: Ak toto nie je k dispozícii alebo je šedý, vyberte **nie** z nižšie uvedených možností prejsť na ďalší krok.</span><span class="sxs-lookup"><span data-stu-id="82f40-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="82f40-115">Pred tým, ako sa tieto zmeny prejavia, môže byť potrebné reštartovať počítač.</span><span class="sxs-lookup"><span data-stu-id="82f40-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="82f40-116">**Odinštalujte a znova nainštalujte ovládač obrazovky:**</span><span class="sxs-lookup"><span data-stu-id="82f40-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="82f40-117">Vyberte položku **Štart**, zadajte **Správca zariadení**a z výsledkov vyberte položku **Správca zariadení** .</span><span class="sxs-lookup"><span data-stu-id="82f40-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="82f40-118">Rozbaľte sekciu **zobrazovacie adaptéry** , kliknite pravým tlačidlom myši na zobrazovací adaptér, ANDS vyberte **odinštalovať zariadenie**.</span><span class="sxs-lookup"><span data-stu-id="82f40-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="82f40-119">Začiarknite políčko vedľa položky **odstrániť softvér ovládača pre toto zariadenie** a vyberte položku **odinštalovať**.</span><span class="sxs-lookup"><span data-stu-id="82f40-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="82f40-120">Poznámka: môže sa zobraziť výzva na reštartovanie počítača v tejto fáze.</span><span class="sxs-lookup"><span data-stu-id="82f40-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="82f40-121">Pred reštartovaním nezabudnite napísať zostávajúce pokyny.</span><span class="sxs-lookup"><span data-stu-id="82f40-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="82f40-122">Znova spustite správcu zariadení.</span><span class="sxs-lookup"><span data-stu-id="82f40-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="82f40-123">Rozbaľte sekciu **zobrazovacie adaptéry** , kliknite pravým tlačidlom myši na zobrazovací adaptér a vyberte položku **aktualizovať ovládač**.</span><span class="sxs-lookup"><span data-stu-id="82f40-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="82f40-124">Vyberte položku **automaticky vyhľadávať aktualizácie softvéru ovládača** a postupujte podľa pokynov na inštaláciu.</span><span class="sxs-lookup"><span data-stu-id="82f40-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>