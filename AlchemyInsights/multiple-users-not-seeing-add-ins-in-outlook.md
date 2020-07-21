---
title: Viacerí používatelia v programe Outlook nevidia doplnky
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198241"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="5164d-102">Viacerí používatelia v programe Outlook nevidia doplnky</span><span class="sxs-lookup"><span data-stu-id="5164d-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="5164d-103">Ak testujete doplnky programu Outlook a žiadne zobraziť, ako prvý krok riešenia problémov, pomocou rutiny cmdlet prostredia PowerShell **Get-OrganizationConfig** dotaz _AppsForOfficeEnabled_ parameter.</span><span class="sxs-lookup"><span data-stu-id="5164d-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="5164d-104">Ak dotaz vráti hodnotu **False**, nastavte tento parameter na **hodnotu True** pomocou rutiny cmdlet **Set-OrganizationConfig,** takže doplnky sa zobrazia podľa očakávania.</span><span class="sxs-lookup"><span data-stu-id="5164d-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="5164d-105">Neodporúčame, aby bol parameter _AppsForOfficeEnabled_ nastavený na **hodnotu False**.</span><span class="sxs-lookup"><span data-stu-id="5164d-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="5164d-106">Hodnota **False** prepíše všetky vyššie uvedené nastavenia správcovskej a používateľskej roly a zabraňuje aktivácii všetkých nových aplikácií ktorýmkoľvek používateľom v organizácii.</span><span class="sxs-lookup"><span data-stu-id="5164d-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="5164d-107">Ďalšie informácie sa nachádzajú v téme [Určenie správcov a používateľov, ktorí môžu inštalovať a spravovať doplnky pre program Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="5164d-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>