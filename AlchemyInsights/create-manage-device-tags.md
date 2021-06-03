---
title: Vytváranie a správa značiek alebo skupín zariadení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731967"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="70b79-102">Vytváranie a správa značiek alebo skupín zariadení</span><span class="sxs-lookup"><span data-stu-id="70b79-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="70b79-103">Pridanie značiek v zariadeniach na vytvorenie logickej závislosti skupiny.</span><span class="sxs-lookup"><span data-stu-id="70b79-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="70b79-104">Značky zariadení podporujú správne mapovanie siete, ktoré vám umožňuje pripojiť rôzne značky na zaznamenanie kontextu a povoliť dynamické vytváranie zoznamu v rámci incidentu.</span><span class="sxs-lookup"><span data-stu-id="70b79-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="70b79-105">Značky možno použiť ako filter v zobrazení zoznamu Zariadenia alebo na zoskupenie zariadení.</span><span class="sxs-lookup"><span data-stu-id="70b79-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="70b79-106">Ďalšie informácie o zoskupovaní zariadení nájdete v téme [Vytvorenie a správa značiek zariadenia.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="70b79-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="70b79-107">Značky v zariadeniach môžete pridať pomocou:</span><span class="sxs-lookup"><span data-stu-id="70b79-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="70b79-108">Používanie portálu</span><span class="sxs-lookup"><span data-stu-id="70b79-108">Using the portal</span></span>

- <span data-ttu-id="70b79-109">Nastavenie hodnoty kľúča databázy Registry</span><span class="sxs-lookup"><span data-stu-id="70b79-109">Setting a registry key value</span></span>
 
<span data-ttu-id="70b79-110">**Poznámka:** Medzi časom pridania značky k zariadeniu a jeho dostupnosťou v zozname zariadení a na stránke zariadenia môže byť časové oneskorenie.</span><span class="sxs-lookup"><span data-stu-id="70b79-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="70b79-111">Ak chcete pridať značky zariadenia pomocou rozhrania API, pozrite si [tému Pridanie alebo odstránenie značky zariadenia API.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="70b79-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="70b79-112">Pridanie a správa značiek zariadení pomocou portálu</span><span class="sxs-lookup"><span data-stu-id="70b79-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="70b79-113">Vyberte zariadenie, v rámci ktorého chcete značky spravovať.</span><span class="sxs-lookup"><span data-stu-id="70b79-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="70b79-114">Zariadenie môžete vybrať alebo vyhľadať v ľubovoľnom z týchto zobrazení:</span><span class="sxs-lookup"><span data-stu-id="70b79-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="70b79-115">**Tabuľa s operáciami zabezpečenia** V časti Najlepšie zariadenia s aktívnymi upozorneniami vyberte názov zariadenia.</span><span class="sxs-lookup"><span data-stu-id="70b79-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="70b79-116">**Front upozornení** – Vyberte názov zariadenia vedľa ikony zariadenia vo fronte upozornení.</span><span class="sxs-lookup"><span data-stu-id="70b79-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="70b79-117">**Zoznam zariadení** – v zozname zariadení vyberte názov zariadenia.</span><span class="sxs-lookup"><span data-stu-id="70b79-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="70b79-118">**Vyhľadávacie pole** – v rozbaľovacej ponuke vyberte položku Zariadenie a zadajte názov zariadenia.</span><span class="sxs-lookup"><span data-stu-id="70b79-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="70b79-119">Na stránku s upozornením môžete prejsť aj cez zobrazenie súborov a IP adries.</span><span class="sxs-lookup"><span data-stu-id="70b79-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="70b79-120">V **riadku akcií** odpovede vyberte položku Spravovať značky.</span><span class="sxs-lookup"><span data-stu-id="70b79-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="70b79-121">Zadajte, či chcete vyhľadať alebo vytvoriť značky.</span><span class="sxs-lookup"><span data-stu-id="70b79-121">Type to find or create tags.</span></span>

<span data-ttu-id="70b79-122">Značky sa pridajú do zobrazenia zariadenia a prejavia sa v zobrazení zoznamu Zariadenia.</span><span class="sxs-lookup"><span data-stu-id="70b79-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="70b79-123">Potom môžete pomocou filtra Značky zobraziť príslušný zoznam zariadení.</span><span class="sxs-lookup"><span data-stu-id="70b79-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="70b79-124">Ďalšie informácie nájdete v téme [Vytvorenie a správa značiek zariadenia.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="70b79-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>