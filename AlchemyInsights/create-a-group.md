---
title: Vytvorenie skupiny
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089175"
---
# <a name="create-a-group"></a><span data-ttu-id="7714f-102">Vytvorenie skupiny</span><span class="sxs-lookup"><span data-stu-id="7714f-102">Create a group</span></span>

<span data-ttu-id="7714f-103">V tejto téme sa popisuje vytváranie skupín.</span><span class="sxs-lookup"><span data-stu-id="7714f-103">This topic describes group creation.</span></span>

<span data-ttu-id="7714f-104">**Povolenie na vytvorenie skupiny**</span><span class="sxs-lookup"><span data-stu-id="7714f-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="7714f-105">Uistite sa, že máte oprávnenie na vytvorenie novej skupiny.</span><span class="sxs-lookup"><span data-stu-id="7714f-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="7714f-106">Globálni správcovia môžu vypnúť vytváranie skupín na portáli Azure alebo v Accessovom paneli.</span><span class="sxs-lookup"><span data-stu-id="7714f-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="7714f-107">Môže byť potrebné, aby správca vytvoril novú skupinu za vás alebo aby vám povolil príslušné povolenia.</span><span class="sxs-lookup"><span data-stu-id="7714f-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="7714f-108">**Správa povolení na vytváranie skupín**</span><span class="sxs-lookup"><span data-stu-id="7714f-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="7714f-109">Globálni správcovia môžu spravovať povolenia na vytváranie skupín (z dôvodov súvisiacich s bezpečnosťou) alebo skupiny služieb Office 365 vytvorené na portáli Azure alebo na prístupovom paneli výberom možnosti používatelia môžu vytvárať skupiny zabezpečenia na azúrových portáloch alebo môžu používatelia 365 vytvárať skupiny v službe Azure Portal vo **všetkých**  >  **všeobecných skupinách (nastavenia)**.</span><span class="sxs-lookup"><span data-stu-id="7714f-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="7714f-110">Môžete tiež obmedziť vytváranie skupín a vybrať skupinu používateľov, ak máte licenciu na Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="7714f-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="7714f-111">**Vypnutie uvítacieho oznámenia pre nových členov skupiny v Office 365**</span><span class="sxs-lookup"><span data-stu-id="7714f-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="7714f-112">Uvítacia notifikácia odoslaná používateľom, ktorí boli pridaní do skupín služieb Office 365, môže byť zakázaná nastavením **UnifiedGroupWelcomeMessageEnabled** na hodnotu False v prostredí PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7714f-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="7714f-113">Oboznámte sa s týmto nastavením [tu](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="7714f-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

