---
title: Používateľovi sa zobrazí chyba AADSTS7000112 Sieť Yammer je vypnutá
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198372"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="f9b13-102">Používateľovi sa zobrazí chyba AADSTS7000112 Sieť Yammer je vypnutá</span><span class="sxs-lookup"><span data-stu-id="f9b13-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="f9b13-103">Ak sa zobrazí chyba "AADSTS7000112: aplikácia "00000005-0000-0ff1-ce00-0000000000000" (Yammer) je vypnutá", existuje problém s hlavné služby azure AD.</span><span class="sxs-lookup"><span data-stu-id="f9b13-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="f9b13-104">Správca mohol vypnúť hlavný server služby blokovať prístup k sieti Yammer.</span><span class="sxs-lookup"><span data-stu-id="f9b13-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="f9b13-105">Vypnutie hlavného nastavenia služby sa neodporúča a môže spôsobiť ďalšie problémy.</span><span class="sxs-lookup"><span data-stu-id="f9b13-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="f9b13-106">Ďalšie informácie o podporovanom prístupe k zablokovaniu prístupu používateľov k yammeru nájdete v téme [Vypnutie prístupu na Yammer pre používateľov služby Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="f9b13-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="f9b13-107">Ak chcete odstrániť tento problém v Azure portál a obnoviť prístup používateľov k sieti Yammer:</span><span class="sxs-lookup"><span data-stu-id="f9b13-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="f9b13-108">Otvorte stránku Azure Active Directory a vyberte **Podnikové aplikácie** podľa **Spravovať** na ľavej navigačnej table.</span><span class="sxs-lookup"><span data-stu-id="f9b13-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="f9b13-109">Do vyhľadávacieho poľa zadajte výraz **Office 365 Yammer** a výberom názvu aplikácie otvorte nastavenia.</span><span class="sxs-lookup"><span data-stu-id="f9b13-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="f9b13-110">Na ľavej navigačnej table vyberte položku **Vlastnosti** v časti **Spravovať.**</span><span class="sxs-lookup"><span data-stu-id="f9b13-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="f9b13-111">Nastavte hodnotu Povolené pre používateľov na **Yes** **prihlásenie?** **Save**</span><span class="sxs-lookup"><span data-stu-id="f9b13-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="f9b13-112">Znova sa prihláste do Yammera.</span><span class="sxs-lookup"><span data-stu-id="f9b13-112">Sign in to Yammer again.</span></span> <span data-ttu-id="f9b13-113">Možno budete musieť vymazať súbory cookie.</span><span class="sxs-lookup"><span data-stu-id="f9b13-113">You might need to clear cookies.</span></span>

<span data-ttu-id="f9b13-114">Prípadne spustite príkazy prostredia PowerShell nastaviť hodnotu.</span><span class="sxs-lookup"><span data-stu-id="f9b13-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="f9b13-115">Ďalšie informácie nájdete v časti ["Ľutujeme, ale máme problémy s prihlásením" chyba pri kliknutí na dlaždicu Yammer v službách Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f9b13-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 