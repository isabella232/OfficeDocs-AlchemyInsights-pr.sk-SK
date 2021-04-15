---
title: 'Chyba: Pravidlá v tomto počítači sa nezhodujú'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782967"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="4f0ba-102">Chyba: Pravidlá v tomto počítači sa nezhodujú</span><span class="sxs-lookup"><span data-stu-id="4f0ba-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="4f0ba-103">Ak chcete zobraziť aktualizovaný stav tohto známeho problému, pozrite si tému Pravidlá v tomto počítači [sa nezhodujú s pravidlami pre Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="4f0ba-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="4f0ba-104">Tím Outlooku implementuje opravu v rámci zostavy 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="4f0ba-105">Oprava sa už nachádza v kanáli Insider Fast a bude sa nachádzať v mesačnom kanáli koncom júna 2020.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="4f0ba-106">Po opravenej zostavy sa môže naposledy zobraziť výzva Ktoré pravidlá si chcete ponechať.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="4f0ba-107">Po zobrazení výzvy vyberte položku Server, vráťte sa do Outlooku a znova zapnite všetky pravidlá, ktoré boli vypnuté.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="4f0ba-108">Kým nebude k dispozícii oprava, použite toto alternatívne riešenie:</span><span class="sxs-lookup"><span data-stu-id="4f0ba-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="4f0ba-109">**Alternatívne** riešenie: V posledných hláseniach sa tento problém vyskytol u používateľov, ktorí si klientske pravidlá vytvárali len v počítačovej aplikácii Outlook.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="4f0ba-110">Ak problém pretrváva, zvážte odstránenie pravidiel a potom pravidlá vytvárajte a upravujte iba v aplikácii OWA (Outlook Web App), kým sa problém nevyrieši.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="4f0ba-111">Ak nie je možné odstrániť pravidlá manuálne, môžete spustiť príkaz programu Outlook pri spustení Outlooku spustením príkazu Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="4f0ba-112">Týmto sa odstránia pravidlá klienta aj servera.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="4f0ba-113">Odstránia sa všetky pravidlá pre všetky kontá v profile Outlooku.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="4f0ba-114">Tento príkaz sa ďalej z dokumentuje v článku Prepínače príkazového riadka.</span><span class="sxs-lookup"><span data-stu-id="4f0ba-114">This command is further documented in the Command-line switches article.</span></span>

