---
title: Diagnostický nástroj služby pre virtuálnu pracovnú plochu Windowsu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596041"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="e41b3-102">Diagnostický nástroj služby pre virtuálnu pracovnú plochu Windowsu</span><span class="sxs-lookup"><span data-stu-id="e41b3-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="e41b3-103">Windows Virtual Desktop (WVD) ponúka diagnostický nástroj, ktorý umožňuje správcom identifikovať chyby prostredníctvom jedného rozhrania.</span><span class="sxs-lookup"><span data-stu-id="e41b3-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="e41b3-104">Tento nástroj zaznamenáva diagnostické informácie vždy, keď WVD použije niekto s priradenou rolou WVD.</span><span class="sxs-lookup"><span data-stu-id="e41b3-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="e41b3-105">Každý denník obsahuje informácie o role WVD, ktorá je súčasťou aktivity, chybových hláseniach, ktoré sa zobrazujú počas relácie, a informácie o nájomníkovi a používateľovi.</span><span class="sxs-lookup"><span data-stu-id="e41b3-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="e41b3-106">Analýzu denníka služby Azure je možné nakonfigurovať na zaznamenávanie denníka aktivít vytvoreného diagnostickým nástrojom pomocou týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="e41b3-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="e41b3-107">Vytvorte pracovný priestor analýzy denníka pomocou portálu [Azure alebo](https://go.microsoft.com/fwlink/?linkid=2129500) prostredia [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="e41b3-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="e41b3-108">[Pripojte počítače s Windowsom k monitoru Azure](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="e41b3-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="e41b3-109">Získajte ID pracovného priestoru a hlavný kľúč pracovného priestoru.</span><span class="sxs-lookup"><span data-stu-id="e41b3-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="e41b3-110">Sprievodca nastavením potrebuje tieto informácie, aby správne nakonfiguroval agenta a zaistil, že bude komunikovať so službou Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="e41b3-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="e41b3-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="e41b3-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="e41b3-112">Diagnostické údaje môžete z nájomníka WVD tlačiť do analýzy denníka svojho pracovného priestoru.</span><span class="sxs-lookup"><span data-stu-id="e41b3-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="e41b3-113">[Identifikujte a diagnostikujte](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problémy, ktoré sú vo vzťahu k WVD interné alebo externé.</span><span class="sxs-lookup"><span data-stu-id="e41b3-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="e41b3-114">Ďalšie informácie o konfigurácii diagnostického nástroja služby pre WVD nájdete v téme Použitie analýzy denníka pre diagnostické funkcie.</span><span class="sxs-lookup"><span data-stu-id="e41b3-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>