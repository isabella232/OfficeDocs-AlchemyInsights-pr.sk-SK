---
title: Reťazec Microsoft Edge User Agent String (pracovná plocha)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679334"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="01033-102">Reťazec Microsoft Edge User Agent String (pracovná plocha)</span><span class="sxs-lookup"><span data-stu-id="01033-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="01033-103">Reťazce User Agent (UA) sa dajú použiť na zistenie, akú verziu konkrétneho prehliadača používate v určitom operačnom systéme.</span><span class="sxs-lookup"><span data-stu-id="01033-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="01033-104">Podobne ako v iných prehliadačoch, Microsoft Edge obsahuje tieto informácie v hlavičke HTTP User-Agent (User-Agent) vždy, keď žiadosť vykoná na lokalite.</span><span class="sxs-lookup"><span data-stu-id="01033-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="01033-105">Prehliadač – informácie o verzii môžete získať aj prostredníctvom JavaScriptu prostredníctvom dotazu na hodnotu "Navigator. userAgent".</span><span class="sxs-lookup"><span data-stu-id="01033-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="01033-106">Odporúčame, aby weboví vývojári využívali funkciu detekcie funkcií vždy, keď je to možné, na zlepšenie údržby kódu, zníženie krehkosti kódu a vylúčenie rizika rozbitia kódu v prípade budúceho aktualizácie reťazcov UA.</span><span class="sxs-lookup"><span data-stu-id="01033-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="01033-107">Ďalšie informácie nájdete v téme [Microsoft Edge User Agent String (Počítačová verzia)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="01033-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>