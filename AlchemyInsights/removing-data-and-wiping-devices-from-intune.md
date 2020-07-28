---
title: Odstránenie údajov a utieranie zariadení z intune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440467"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="dc0e4-102">Odstránenie údajov a utieranie zariadení z intune</span><span class="sxs-lookup"><span data-stu-id="dc0e4-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="dc0e4-103">Vzdialené akcie Zariadenia v režime odchodu do dôchodku a Vymazanie zariadení možno použiť na odstránenie údajov spoločnosti spravovaných spoločnosťou Intune alebo na obnovenie výrobných nastavení a vrátenie zariadenia do predvolených nastavení.</span><span class="sxs-lookup"><span data-stu-id="dc0e4-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="dc0e4-104">Prihláste sa do služby Správa zariadení od spoločnosti Microsoft 365 a prejdite do ponuky **Devices**  >  **All Devices (Všetky zariadenia).**</span><span class="sxs-lookup"><span data-stu-id="dc0e4-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="dc0e4-105">Vyberte zariadenie, ktoré chcete vymazať.</span><span class="sxs-lookup"><span data-stu-id="dc0e4-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="dc0e4-106">Vyberte typ vzdialeného vymazania, ktoré chcete urobiť.</span><span class="sxs-lookup"><span data-stu-id="dc0e4-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="dc0e4-107">Odchod do dôchodku odstráni iba organizačné informácie, zatiaľ čo úplné vymazanie obnoví výrobné nastavenia zariadenia.</span><span class="sxs-lookup"><span data-stu-id="dc0e4-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="dc0e4-108">Výber **potvrďte výberom** položky Yes (Áno).</span><span class="sxs-lookup"><span data-stu-id="dc0e4-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="dc0e4-109">Kým vymazanie skončí, stav akcie zariadenie sa zobrazí ako Odchod do dôchodku čakajúce.</span><span class="sxs-lookup"><span data-stu-id="dc0e4-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="dc0e4-110">Po dokončení akcie sa mobilné zariadenie už nebude nachádzať v zozname spravovaných zariadení.</span><span class="sxs-lookup"><span data-stu-id="dc0e4-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="dc0e4-111">**Upozornenie:** Údaje spoločnosti nie je možné odstrániť zo zariadení pripojených k službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dc0e4-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="dc0e4-112">Podrobné informácie o účinku akcií Odísť do dôchodku a Vymazanie vrátane toho, čo sa zachová a čo sa odstráni, nájdete [v téme Odstránenie zariadení pomocou vymazania, odchodu do dôchodku alebo manuálneho zrušenia zariadenia](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="dc0e4-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="dc0e4-113">Ak chcete vymazať všetky údaje zo zariadenia so systémom macOS, pozrite [si tému Vymazanie všetkých údajov zo zariadenia so systémom macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="dc0e4-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>