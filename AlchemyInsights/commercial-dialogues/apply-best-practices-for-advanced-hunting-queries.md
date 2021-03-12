---
title: Použitie najvhodnejších postupov pri rozšírených dotazoch na lov
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749548"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="2a502-102">Použitie najvhodnejších postupov pri rozšírených dotazoch na lov</span><span class="sxs-lookup"><span data-stu-id="2a502-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="2a502-103">Ak chcete rýchlejšie získavať výsledky a vyhnúť sa timeoutom pri spúšťaní zložitých dotazov, použite tieto najvhodnejšie postupy:</span><span class="sxs-lookup"><span data-stu-id="2a502-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="2a502-104">Pri pokuse o nové dotazy vždy použite limit, aby sa predišlo extrémne vysokým množinám výsledkov.</span><span class="sxs-lookup"><span data-stu-id="2a502-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="2a502-105">Môžete tiež použiť `count` na vytvorenie počiatočného hodnotenia veľkosti množiny výsledkov.</span><span class="sxs-lookup"><span data-stu-id="2a502-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="2a502-106">Najprv použite časové filtre.</span><span class="sxs-lookup"><span data-stu-id="2a502-106">Use time filters first.</span></span> <span data-ttu-id="2a502-107">V ideálnom prípade Obmedzte dotazy na sedem dní.</span><span class="sxs-lookup"><span data-stu-id="2a502-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="2a502-108">Na začiatku dotazu, hneď po uplynutí časového filtra, pridajte filtre, ktoré sa očakávajú na odstránenie väčšiny údajov.</span><span class="sxs-lookup"><span data-stu-id="2a502-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="2a502-109">Pri vyhľadávaní úplných tokenov použite `has` operátor skôr ako `contains` .</span><span class="sxs-lookup"><span data-stu-id="2a502-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="2a502-110">Spustite vyhľadávanie v konkrétnom stĺpci a nie vo všetkých stĺpcoch.</span><span class="sxs-lookup"><span data-stu-id="2a502-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="2a502-111">Pri pripájaní k tabuľkám najskôr zadajte tabuľku s menším počtom riadkov.</span><span class="sxs-lookup"><span data-stu-id="2a502-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="2a502-112">`project` iba potrebné stĺpce z tabuliek, ku ktorým ste sa pripojili.</span><span class="sxs-lookup"><span data-stu-id="2a502-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="2a502-113">Ďalšie informácie nájdete v téme [pokročilé postupy lovu v dotaze](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="2a502-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
