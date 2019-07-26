---
title: Zmena názvových serverov
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902944"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="429bc-102">Aktualizácia názvových serverov domény v službách Office 365</span><span class="sxs-lookup"><span data-stu-id="429bc-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="429bc-103">Poznámka: Rozšírenie zmien názvových serverov môže trvať až 48 hodín.</span><span class="sxs-lookup"><span data-stu-id="429bc-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="429bc-104">Ak chcete nastaviť doménu v službách Office 365, názvové servery u vášho registrátora musia byť aktualizované.</span><span class="sxs-lookup"><span data-stu-id="429bc-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="429bc-105">Vytvorte alebo upravte záznamy názvového servera u registrátora domén.</span><span class="sxs-lookup"><span data-stu-id="429bc-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="429bc-106">Prejdite na webovú lokalitu registrátora domén a vyhľadajte miesto, kde môžete upraviť názvové servery.</span><span class="sxs-lookup"><span data-stu-id="429bc-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="429bc-107">Vytvorte alebo upravte dva záznamy názvového servera, ktoré sa zhodujú s týmito hodnotami:</span><span class="sxs-lookup"><span data-stu-id="429bc-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="429bc-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="429bc-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="429bc-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="429bc-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="429bc-110">Uložte zmeny.</span><span class="sxs-lookup"><span data-stu-id="429bc-110">Save changes.</span></span>

<span data-ttu-id="429bc-111">Podrobné pokyny nájdete aj v tomto článku: [Zmena názvových serverov na nastavenie služieb Office 365 s ľubovoľným registrátorom domén](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="429bc-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  