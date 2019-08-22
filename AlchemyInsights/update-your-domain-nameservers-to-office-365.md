---
title: Aktualizácia názvových serverov domény v službách Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 2447a3300782204b32d3c47325e1e987f6168be7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506062"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="af93e-102">Aktualizácia názvových serverov domény v službách Office 365</span><span class="sxs-lookup"><span data-stu-id="af93e-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="af93e-103">Poznámka: Rozšírenie zmien názvových serverov môže trvať až 48 hodín.</span><span class="sxs-lookup"><span data-stu-id="af93e-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="af93e-104">Ak chcete nastaviť doménu v službách Office 365, názvové servery u vášho registrátora musia byť aktualizované.</span><span class="sxs-lookup"><span data-stu-id="af93e-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="af93e-105">Vytvorte alebo upravte záznamy názvového servera u registrátora domén.</span><span class="sxs-lookup"><span data-stu-id="af93e-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="af93e-106">Prejdite na webovú lokalitu registrátora domén a vyhľadajte miesto, kde môžete upraviť názvové servery.</span><span class="sxs-lookup"><span data-stu-id="af93e-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="af93e-107">Vytvorte alebo upravte dva záznamy názvového servera, ktoré sa zhodujú s týmito hodnotami:</span><span class="sxs-lookup"><span data-stu-id="af93e-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="af93e-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="af93e-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="af93e-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="af93e-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="af93e-110">Uložte zmeny.</span><span class="sxs-lookup"><span data-stu-id="af93e-110">Save changes.</span></span>

<span data-ttu-id="af93e-111">Podrobné pokyny nájdete aj v tomto článku: [Zmena názvových serverov na nastavenie služieb Office 365 s ľubovoľným registrátorom domén](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="af93e-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  