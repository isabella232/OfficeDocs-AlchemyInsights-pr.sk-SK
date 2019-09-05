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
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742201"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="03666-102">Aktualizácia názvových serverov domény v službách Office 365</span><span class="sxs-lookup"><span data-stu-id="03666-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="03666-103">Poznámka: Rozšírenie zmien názvových serverov môže trvať až 48 hodín.</span><span class="sxs-lookup"><span data-stu-id="03666-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="03666-104">Ak chcete nastaviť doménu v službách Office 365, názvové servery u vášho registrátora musia byť aktualizované.</span><span class="sxs-lookup"><span data-stu-id="03666-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="03666-105">Vytvorte alebo upravte záznamy názvového servera u registrátora domén.</span><span class="sxs-lookup"><span data-stu-id="03666-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="03666-106">Prejdite na webovú lokalitu registrátora domén a vyhľadajte miesto, kde môžete upraviť názvové servery.</span><span class="sxs-lookup"><span data-stu-id="03666-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="03666-107">Vytvorte alebo upravte dva záznamy názvového servera, ktoré sa zhodujú s týmito hodnotami:</span><span class="sxs-lookup"><span data-stu-id="03666-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="03666-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="03666-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="03666-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="03666-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="03666-110">Uložte zmeny.</span><span class="sxs-lookup"><span data-stu-id="03666-110">Save changes.</span></span>

<span data-ttu-id="03666-111">Podrobné pokyny nájdete aj v tomto článku: [Zmena názvových serverov na nastavenie služieb Office 365 s ľubovoľným registrátorom domén](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="03666-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  