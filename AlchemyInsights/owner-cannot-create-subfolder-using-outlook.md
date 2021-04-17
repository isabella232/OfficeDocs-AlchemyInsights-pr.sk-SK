---
title: Vlastník nemôže vytvoriť pod priečinok pomocou programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836150"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="3dc9d-102">Vlastník nemôže vytvoriť pod priečinok pomocou programu Outlook</span><span class="sxs-lookup"><span data-stu-id="3dc9d-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="3dc9d-103">**Priebežne sa vyskytuje problém, ktorý sa vyskytuje pri vytváraní podpriečinkov vlastníkmi verejných priečinkov pomocou Outlooku. Problém sa čoskoro opraví.**</span><span class="sxs-lookup"><span data-stu-id="3dc9d-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="3dc9d-104">Zatiaľ použite niektoré z nasledujúcich alternatívnych riešení:</span><span class="sxs-lookup"><span data-stu-id="3dc9d-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="3dc9d-105">Pomocou Outlooku pre MAC vytvorte podpriečinok, keďže problém ovplyvňuje iba Outlook pre stolné okná (všetky verzie)</span><span class="sxs-lookup"><span data-stu-id="3dc9d-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="3dc9d-106">Správca môže vytvoriť podpriečinok pomocou prostredia EXO Shell alebo EAC</span><span class="sxs-lookup"><span data-stu-id="3dc9d-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="3dc9d-107">Zmena priečinka DefaultPublicFolderMailbox/EffectivePublicFolderMailbox používateľa na inú poštovú schránku ako poštovú schránku obsahu, ktorá spôsobuje problém</span><span class="sxs-lookup"><span data-stu-id="3dc9d-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="3dc9d-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="3dc9d-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="3dc9d-109">Počkajte jednu hodinu a reštartujte klienta Outlooku</span><span class="sxs-lookup"><span data-stu-id="3dc9d-109">Wait for an hour, restart outlook client</span></span>