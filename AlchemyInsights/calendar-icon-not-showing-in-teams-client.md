---
title: Ikona kalendára sa nezobrazuje v klientovi aplikácie Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819968"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="fda3c-102">Ikona kalendára sa nezobrazuje v klientovi aplikácie Teams</span><span class="sxs-lookup"><span data-stu-id="fda3c-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="fda3c-103">Karta Kalendár v aplikácii Teams vyžaduje prístup do exchangeovej poštovej schránky prostredníctvom webových služieb Exchangeu.</span><span class="sxs-lookup"><span data-stu-id="fda3c-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="fda3c-104">Exchangeová poštová schránka môže byť online alebo lokálna.</span><span class="sxs-lookup"><span data-stu-id="fda3c-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="fda3c-105">Ak sa online používateľom nezobrazuje karta Kalendár, uistite sa, že [majú licenciu na exchangeovú online poštovú schránku a poštová schránka je povolená](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="fda3c-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="fda3c-106">Ak má používateľ platnú poštovú schránku v službe Exchange Online, ale stále sa nezobrazuje karta Kalendár, pravdepodobne sa vyskytol problém so sieťou.</span><span class="sxs-lookup"><span data-stu-id="fda3c-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="fda3c-107">Použite [nástroj Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) a spustite **testovanie pripojenia vo webových službách Microsoft Exchangeu** pre daného používateľa.</span><span class="sxs-lookup"><span data-stu-id="fda3c-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="fda3c-108">Nakoniec skontrolujte [pre aplikácie Teams politiky nastavenia aplikácií](https://admin.teams.microsoft.com/policies/app-setup) a skontrolujte, či aplikácia Kalendár nebola odobratá z politiky, ktorá sa použila pre daného používateľa (s najväčšou pravdepodobnosťou sú to politiky **globálne (predvolené pre celú organizáciu)**.</span><span class="sxs-lookup"><span data-stu-id="fda3c-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="fda3c-109">Ak sú poštové schránky vašich používateľov lokálne, je potrebné potvrdiť, že je stav vašej hybridnej konfigurácie v poriadku.</span><span class="sxs-lookup"><span data-stu-id="fda3c-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="fda3c-110">Ak chcete riešiť problémy, použite [Sprievodcu hybridnou konfiguráciou](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="fda3c-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="fda3c-111">Upozorňujeme, že [aplikácia Teams vyžaduje Exchange 2016 CU3 alebo novší](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="fda3c-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
