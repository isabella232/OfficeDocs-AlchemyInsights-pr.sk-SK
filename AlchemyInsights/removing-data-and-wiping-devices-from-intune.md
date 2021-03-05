---
title: Odstránenie údajov a vymazanie zariadení z Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416328"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="95a71-102">Odstránenie údajov a vymazanie zariadení z Intune</span><span class="sxs-lookup"><span data-stu-id="95a71-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="95a71-103">Vzdialené akcie Vyradenie zariadenia a Vymazanie zariadenia možno použiť na odstránenie podnikových údajov spravovaných službou Intune alebo na resetovanie výrobných nastavení a obnovenie predvolených nastavení zariadenia.</span><span class="sxs-lookup"><span data-stu-id="95a71-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="95a71-104">Prihláste sa do aplikácie Správa zariadení pre Microsoft 365 a prejdite na položku **Zariadenia** > **Všetky zariadenia**.</span><span class="sxs-lookup"><span data-stu-id="95a71-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="95a71-105">Vyberte zariadenie, v ktorom chcete údaje vymazať.</span><span class="sxs-lookup"><span data-stu-id="95a71-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="95a71-106">Vyberte požadovaný typ vzdialeného vymazania údajov.</span><span class="sxs-lookup"><span data-stu-id="95a71-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="95a71-107">Možnosť vyradenia odstráni len informácie organizácie, zatiaľ čo úplné vymazanie údajov obnoví výrobné nastavenia zariadenia.</span><span class="sxs-lookup"><span data-stu-id="95a71-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="95a71-108">Výber potvrďte kliknutím na tlačidlo **Áno**.</span><span class="sxs-lookup"><span data-stu-id="95a71-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="95a71-109">Kým sa vymazanie nedokončí, stav akcie Zariadenie sa zobrazuje ako *Čaká sa na vyradenie*.</span><span class="sxs-lookup"><span data-stu-id="95a71-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="95a71-110">Po dokončení akcie sa mobilné zariadenie už v zozname spravovaných zariadení nebude nachádzať.</span><span class="sxs-lookup"><span data-stu-id="95a71-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="95a71-111">Údaje spoločnosti nie je možné odstrániť zo zariadení PRIPOJENÝCH do služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="95a71-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="95a71-112">Úplné podrobnosti o vplyve akcií Vyradeniie a Vymazanie vrátane toho, čo sa zachová a čo sa odstráni, nájdete v nasledujúcej dokumentácii:</span><span class="sxs-lookup"><span data-stu-id="95a71-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="95a71-113">[Odstránenie zariadení pomocou vymazania, vyradenia alebo manuálneho zrušenia registrácie](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="95a71-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="95a71-114">Vymazanie len podnikových údajov z aplikácií spravovaných službou Intune</span><span class="sxs-lookup"><span data-stu-id="95a71-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="95a71-115">[Vymazanie všetkých údajov zo zariadenia so systémom macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="95a71-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>