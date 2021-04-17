---
title: Vytvorenie skupiny
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816387"
---
# <a name="create-a-group"></a><span data-ttu-id="0eb4e-102">Vytvorenie skupiny</span><span class="sxs-lookup"><span data-stu-id="0eb4e-102">Create a group</span></span>

<span data-ttu-id="0eb4e-103">Táto téma popisuje vytváranie skupín.</span><span class="sxs-lookup"><span data-stu-id="0eb4e-103">This topic describes group creation.</span></span>

<span data-ttu-id="0eb4e-104">**Povolenie na vytvorenie skupiny**</span><span class="sxs-lookup"><span data-stu-id="0eb4e-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="0eb4e-105">Uistite sa, že máte oprávnenie vytvoriť novú skupinu.</span><span class="sxs-lookup"><span data-stu-id="0eb4e-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="0eb4e-106">Globálni správcovia môžu zakázať vytváranie skupín na portáli Azure alebo na paneli prístupu.</span><span class="sxs-lookup"><span data-stu-id="0eb4e-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="0eb4e-107">Na vytvorenie novej skupiny alebo na zadanie príslušných povolení budete možno potrebovať správcu.</span><span class="sxs-lookup"><span data-stu-id="0eb4e-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="0eb4e-108">**Správa povolení na vytváranie skupín**</span><span class="sxs-lookup"><span data-stu-id="0eb4e-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="0eb4e-109">Globálni správcovia môžu spravovať povolenia na vytváranie skupín (z dôvodov zabezpečenia) alebo skupiny v Office 365 vytvorené na portáli Azure alebo na prístupnom paneli výberom možnosti Používatelia môžu vytvárať skupiny zabezpečenia na portáloch Azure alebo Možnosti Používatelia môžu vytvárať skupiny v Office 365 na portáloch Azure vo všetkých skupinách  >  **Všeobecné (Nastavenia).**</span><span class="sxs-lookup"><span data-stu-id="0eb4e-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="0eb4e-110">Môžete tiež obmedziť vytváranie skupín a vybrať skupinu používateľov, ak máte licenciu na Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="0eb4e-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="0eb4e-111">**Vypnutie uvítacej oznámenia pre nových členov skupiny v Office 365**</span><span class="sxs-lookup"><span data-stu-id="0eb4e-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="0eb4e-112">Uvítacie oznámenie odoslané používateľom, ktorí sú pridaní do skupín v Office 365, možno vypnúť nastavením možnosti **UnifiedGroupWelcomeMessageEnabled** na hodnotu False v prostredí Powershell.</span><span class="sxs-lookup"><span data-stu-id="0eb4e-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="0eb4e-113">Informácie o tomto nastavení nájdete [tu.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="0eb4e-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

