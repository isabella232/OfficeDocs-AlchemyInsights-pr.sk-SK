---
title: Nástroj na diagnostiku služby pre virtuálnu pracovnú plochu Windowsu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680231"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="c181d-102">Nástroj na diagnostiku služby pre virtuálnu pracovnú plochu Windowsu</span><span class="sxs-lookup"><span data-stu-id="c181d-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="c181d-103">Windows Virtual Desktop (WVD) ponúka diagnostický nástroj, ktorý umožňuje správcom identifikovať chyby prostredníctvom jedného rozhrania.</span><span class="sxs-lookup"><span data-stu-id="c181d-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="c181d-104">Tento nástroj zapisuje informácie súvisiace s diagnostikou pri každom použití WVD používateľom priradenej roly WVD.</span><span class="sxs-lookup"><span data-stu-id="c181d-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="c181d-105">Každý denník obsahuje informácie o WVD úlohe zahrnutej v aktivite, chybových správach, ktoré sa zobrazujú počas relácie, a informácie o nájomníkovi a používateľovi.</span><span class="sxs-lookup"><span data-stu-id="c181d-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="c181d-106">Analýzu denníka služby Azure je možné nakonfigurovať tak, aby zaznamenávala denník aktivít vytvorený diagnostickým nástrojom.</span><span class="sxs-lookup"><span data-stu-id="c181d-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="c181d-107">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="c181d-107">Here's how:</span></span>

1. <span data-ttu-id="c181d-108">Vytvorenie pracovného priestoru denníka analýzy pomocou [portálu Azure](https://go.microsoft.com/fwlink/?linkid=2129500) alebo [prostredia Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="c181d-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="c181d-109">[Pripojte počítače s Windowsom k službe Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="c181d-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="c181d-110">Získajte identifikáciu pracovného priestoru a hlavný kľúč pracovného priestoru.</span><span class="sxs-lookup"><span data-stu-id="c181d-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="c181d-111">Sprievodca nastavením vyžaduje, aby tieto informácie správne nakonfigurovali agenta a zaistili, že dokážu komunikovať so službou Azure monitor.</span><span class="sxs-lookup"><span data-stu-id="c181d-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="c181d-112">[Vytlačte údaje diagnostiky do pracovného priestoru](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="c181d-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="c181d-113">Údaje o diagnostike môžete tlačiť z nájomníka WVD do denníka Analytics pre váš pracovný priestor.</span><span class="sxs-lookup"><span data-stu-id="c181d-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="c181d-114">[Identifikujte a diagnostikujte problémy](https://go.microsoft.com/fwlink/?linkid=2128338) , ktoré sú interné alebo externé vo vzťahu k WVD.</span><span class="sxs-lookup"><span data-stu-id="c181d-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="c181d-115">Ďalšie informácie o konfigurácii nástroja Diagnostika služby pre WVD nájdete v téme [použitie funkcie Denníková analýza pre funkciu diagnostiky](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="c181d-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
