---
title: Nastavenie Microsoft Edgeu ako predvoleného prehliadača v zariadení s doménou
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491879"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="db201-102">Nastavenie Microsoft Edgeu ako predvoleného prehliadača v zariadení s doménou</span><span class="sxs-lookup"><span data-stu-id="db201-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="db201-103">Nastavte Microsoft Edge ako predvolený prehliadač:</span><span class="sxs-lookup"><span data-stu-id="db201-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="db201-104">[Vytvorte súbor predvolenej konfigurácie priradenia a](https://go.microsoft.com/fwlink/?linkid=2132437) uložte ho lokálne alebo v zdieľanom mieste v sieti.</span><span class="sxs-lookup"><span data-stu-id="db201-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="db201-105">Otvorte editor skupinovej politiky a potom prejdite na položku Šablóny na správu **konfigurácie**  >  **počítača, Prieskumník** súčasti  >  **systému Windows.**  >  </span><span class="sxs-lookup"><span data-stu-id="db201-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="db201-106">Vyberte **položku Nastaviť predvolený konfiguračný súbor priradení.**</span><span class="sxs-lookup"><span data-stu-id="db201-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="db201-107">Vyberte **položku Nastavenie politiky** a potom položku **Povolené**.</span><span class="sxs-lookup"><span data-stu-id="db201-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="db201-108">V **časti** Možnosti zadajte umiestnenie predvoleného konfiguračného súboru priradení a potom vyberte tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="db201-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
