---
title: Používanie aplikácie TeamViewer na vzdialenú správu zariadení Intune
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
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555749"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="3df3e-102">Používanie aplikácie TeamViewer na vzdialenú správu zariadení Intune</span><span class="sxs-lookup"><span data-stu-id="3df3e-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="3df3e-103">Zariadenia spravované aplikáciou Intune je možné spravovať na diaľku pomocou [aplikácie TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="3df3e-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="3df3e-104">Ak chcete spravovať aplikáciu Intune pomocou aplikácie TeamViewer, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="3df3e-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="3df3e-105">Začnite získaním poverení z aplikácie TeamViewer na nastavenie konektora TeamViewer v programe Intune.</span><span class="sxs-lookup"><span data-stu-id="3df3e-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="3df3e-106">To umožňuje správcovi zadať poverenia v používateľskom rozhraní konektora TeamViewer v časti Zariadenia, čo je jednorázová operácia na vytvorenie prepojenia medzi intune a službou TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="3df3e-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="3df3e-107">**Časť 1: Spustenie relácie so vzdialeným zariadením**</span><span class="sxs-lookup"><span data-stu-id="3df3e-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="3df3e-108">V **časti Všetky**zariadenia vyberte zariadenie, s ktorými chcete spustiť vzdialenú reláciu.</span><span class="sxs-lookup"><span data-stu-id="3df3e-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="3df3e-109">Od **... 3/4e**vyberte **Nová relácia pomoci na diaľku**.</span><span class="sxs-lookup"><span data-stu-id="3df3e-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="3df3e-110">Ak chcete **potvrdiť,** že chcete vytvoriť vzdialenú reláciu, vyberte možnosť Áno.</span><span class="sxs-lookup"><span data-stu-id="3df3e-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="3df3e-111">Po tom, ako služba TeamViewer potvrdí žiadosť "Inicializácia novej vzdialenej **Start remote assistance** relácie", sa na table Prehľad (alebo Essentials) zariadenia zobrazí možnosť Spustiť pomoc na diaľku.</span><span class="sxs-lookup"><span data-stu-id="3df3e-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="3df3e-112">Výberom **položky Zobraziť ďalšie** rozbaľte tablu a zobrazte stav Pomoci na diaľku.</span><span class="sxs-lookup"><span data-stu-id="3df3e-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="3df3e-113">Výberom **položky Spustiť vzdialenú** reláciu spustite reláciu na strane správcu.</span><span class="sxs-lookup"><span data-stu-id="3df3e-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="3df3e-114">Vyberte, či chcete stiahnuť binárny súbor aplikácie TeamViewer (Windows) a vyberte položku **Spustiť**.</span><span class="sxs-lookup"><span data-stu-id="3df3e-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="3df3e-115">**Upozornenie:** Môžete ignorovať ľubovoľnú stránku webového prehľadávača otvorenú na webovej lokalite aplikácie TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="3df3e-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="3df3e-116">Potvrďte žiadosť o aplikáciu TeamViewer na zmeny v zariadení (len v systéme Windows).</span><span class="sxs-lookup"><span data-stu-id="3df3e-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="3df3e-117">Spustí sa aplikácia TeamViewer a obsahuje kód relácie na overenie pripojenia k vzdialenému zariadeniu.</span><span class="sxs-lookup"><span data-stu-id="3df3e-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="3df3e-118">**Časť 2: Na zariadení, ktoré je určené na vzdialenú reláciu**</span><span class="sxs-lookup"><span data-stu-id="3df3e-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="3df3e-119">Otvorte portál spoločnosti Intune.</span><span class="sxs-lookup"><span data-stu-id="3df3e-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="3df3e-120">Vyhľadajte príznak upozornenia: "Správca IT požaduje kontrolu nad týmto zariadením pre reláciu pomoci na diaľku a vyberte upozornenie.</span><span class="sxs-lookup"><span data-stu-id="3df3e-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="3df3e-121">Vyberte, či chcete stiahnuť aplikáciu TeamViewer, alebo potvrďte stiahnutie aplikácie TeamViewer z obchodu s aplikáciami a vyberte položku **Spustiť**.</span><span class="sxs-lookup"><span data-stu-id="3df3e-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="3df3e-122">**Upozornenie:** Môžete ignorovať ľubovoľnú stránku webového prehľadávača otvorenú na webovej lokalite aplikácie TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="3df3e-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="3df3e-123">Potvrďte žiadosť o aplikáciu TeamViewer na zmeny v zariadení (len v systéme Windows).</span><span class="sxs-lookup"><span data-stu-id="3df3e-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="3df3e-124">Spustí sa aplikácia TeamViewer a obsahuje kód relácie na overenie pripojenia k vzdialenému zariadeniu.</span><span class="sxs-lookup"><span data-stu-id="3df3e-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="3df3e-125">Kontextová ponuka sa zobrazí otázka, či chcete povoliť spustenie relácie.</span><span class="sxs-lookup"><span data-stu-id="3df3e-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="3df3e-126">**Upozornenie:** Kódy relácií generované službou TeamViewer sú len na jedno použitie.</span><span class="sxs-lookup"><span data-stu-id="3df3e-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="3df3e-127">Ak stratíte pripojenie, musíte:</span><span class="sxs-lookup"><span data-stu-id="3df3e-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="3df3e-128">Zatvorte inštanciu aplikácie TeamViewer na vzdialenom zariadení a na pracovnej stanici správcu.</span><span class="sxs-lookup"><span data-stu-id="3df3e-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="3df3e-129">Zatvorte firemný portál na vzdialenom zariadení.</span><span class="sxs-lookup"><span data-stu-id="3df3e-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="3df3e-130">Inicializovať novú "Novú reláciu pomoci na diaľku" z portálu na správu.</span><span class="sxs-lookup"><span data-stu-id="3df3e-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="3df3e-131">Znova otvorte firemný portál na vzdialenom zariadení a dostanete nové upozornenie.</span><span class="sxs-lookup"><span data-stu-id="3df3e-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="3df3e-132">Stiahnite si a otvorte aplikáciu TeamViewer na vzdialenom zariadení aj na pracovnej stanici správcu, ako predtým.</span><span class="sxs-lookup"><span data-stu-id="3df3e-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>