---
title: Vlastník nemôže vytvoriť podpriečinok s použitím Outlooku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665733"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="94368-102">Vlastník nemôže vytvoriť podpriečinok s použitím Outlooku</span><span class="sxs-lookup"><span data-stu-id="94368-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="94368-103">**Vyskytol sa problém s vlastníkmi verejných priečinkov vytvárajúcich podpriečinky pomocou Outlooku. Tento problém bude čoskoro vyriešený.**</span><span class="sxs-lookup"><span data-stu-id="94368-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="94368-104">Zatiaľ použite jeden z nasledujúcich postupov:</span><span class="sxs-lookup"><span data-stu-id="94368-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="94368-105">Použitie Outlooku pre MAC na vytvorenie podpriečinka ako problém ovplyvňuje len Outlook pre stolné počítače (všetky verzie)</span><span class="sxs-lookup"><span data-stu-id="94368-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="94368-106">Požiadajte správcu o vytvorenie podpriečinka s použitím EXO shellu alebo EAC</span><span class="sxs-lookup"><span data-stu-id="94368-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="94368-107">Zmena DefaultPublicFolderMailbox/EffectivePublicFolderMailbox používateľa na inú poštovú schránku, než je poštová schránka obsahu priečinka spôsobujúceho problém</span><span class="sxs-lookup"><span data-stu-id="94368-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="94368-108">*Množina poštových schránok user1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="94368-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="94368-109">Počkať na hodinu, reštartujte klienta Outlook</span><span class="sxs-lookup"><span data-stu-id="94368-109">Wait for an hour, restart outlook client</span></span>