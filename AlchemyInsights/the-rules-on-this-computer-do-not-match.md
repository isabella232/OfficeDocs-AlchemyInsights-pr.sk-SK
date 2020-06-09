---
title: 'Chyba: Pravidlá v tomto počítači sa nezhodujú'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618028"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="684c4-102">Chyba: Pravidlá v tomto počítači sa nezhodujú</span><span class="sxs-lookup"><span data-stu-id="684c4-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="684c4-103">Ak chcete zobraziť aktualizovaný stav tohto známeho problému, pozrite [si pravidlá v tomto počítači nezodpovedajú pravidlám na serveri Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="684c4-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="684c4-104">Tím programu Outlook implementoval opravu v build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="684c4-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="684c4-105">Oprava je už na Insider Fast a pôjde do mesačného kanála na konci júna 2020.</span><span class="sxs-lookup"><span data-stu-id="684c4-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="684c4-106">Akonáhle budete mať pevnú stavať môžete dostať výzvu "Aké pravidlá chcete zachovať" ešte raz.</span><span class="sxs-lookup"><span data-stu-id="684c4-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="684c4-107">Po zobrazení výzvy vyberte položku Server a potom sa vráťte do programu Outlook a znova povoľte všetky pravidlá, ktoré boli vypnuté.</span><span class="sxs-lookup"><span data-stu-id="684c4-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="684c4-108">Kým oprava je k dispozícii, použite nasledujúce riešenie:</span><span class="sxs-lookup"><span data-stu-id="684c4-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="684c4-109">**Riešenie:** V posledných zostavách sa vyskytol problém pre tých, ktorí vytvorili iba pravidlá klienta v pracovnej ploche programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="684c4-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="684c4-110">Ak sa problém vyskytuje aj naďalej, zvážte odstránenie pravidiel a potom vytvorte a upravte pravidlá iba v aplikácii OWA (Outlook Web App), kým sa problém nevyrieši.</span><span class="sxs-lookup"><span data-stu-id="684c4-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="684c4-111">Ak nemôžete odstrániť pravidlá manuálne, môžete spustiť príkaz programu Outlook pri spustení programu Outlook spustením outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="684c4-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="684c4-112">Tým sa odstránia pravidlá klienta aj servera.</span><span class="sxs-lookup"><span data-stu-id="684c4-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="684c4-113">Odstráni všetky pravidlá pre všetky kontá v profile programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="684c4-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="684c4-114">Tento príkaz je ďalej zdokumentovaný v článku prepínače príkazového riadka.</span><span class="sxs-lookup"><span data-stu-id="684c4-114">This command is further documented in the Command-line switches  article.</span></span>