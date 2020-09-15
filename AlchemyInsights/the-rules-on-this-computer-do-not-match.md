---
title: 'Chyba: pravidlá v tomto počítači sa nezhodujú'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690978"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="8e108-102">Chyba: pravidlá v tomto počítači sa nezhodujú</span><span class="sxs-lookup"><span data-stu-id="8e108-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="8e108-103">Ak chcete zobraziť aktualizovaný stav tohto známeho problému, pozrite si tému [pravidlá v tomto počítači sa nezhodujú s pravidlami na serveri Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="8e108-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="8e108-104">Tím Outlooku implementoval opravu v zostave 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="8e108-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="8e108-105">Oprava je už na lokalite Insider Fast a prechod na mesačný kanál sa koncom júna 2020.</span><span class="sxs-lookup"><span data-stu-id="8e108-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="8e108-106">Po vytvorení pevnej zostavy sa môže zobraziť výzva "ktoré pravidlá si chcete ponechať" naposledy.</span><span class="sxs-lookup"><span data-stu-id="8e108-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="8e108-107">Po zobrazení výzvy vyberte položku Server a potom sa vráťte späť v Outlooku a znova zapnite všetky pravidlá, ktoré boli vypnuté.</span><span class="sxs-lookup"><span data-stu-id="8e108-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="8e108-108">Kým nie je k dispozícii oprava, použite toto alternatívne riešenie:</span><span class="sxs-lookup"><span data-stu-id="8e108-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="8e108-109">**Alternatívne riešenie**: v nedávnych zostavách sa vyskytol problém pre tých, ktorí vytvorili len pravidlá klienta v počítačovej verzii Outlooku.</span><span class="sxs-lookup"><span data-stu-id="8e108-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="8e108-110">Ak sa problém vyskytuje aj naďalej, zvážte odstránenie pravidiel a potom vytváranie a úprava pravidiel len v aplikácii OWA (Outlook Web App) dovtedy, kým sa problém nevyrieši.</span><span class="sxs-lookup"><span data-stu-id="8e108-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="8e108-111">Ak nemôžete odstrániť pravidlá manuálne môžete spustiť Outlook príkaz pri spustení Outlooku spustením Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="8e108-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="8e108-112">Týmto sa odstránia pravidlá klienta aj servera.</span><span class="sxs-lookup"><span data-stu-id="8e108-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="8e108-113">Odstránia sa všetky pravidlá pre všetky kontá v profile programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="8e108-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="8e108-114">Tento príkaz je ďalej zdokumentovaný v článku prepínače príkazového tlačidla.</span><span class="sxs-lookup"><span data-stu-id="8e108-114">This command is further documented in the Command-line switches article.</span></span>

