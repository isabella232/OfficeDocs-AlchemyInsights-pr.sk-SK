---
title: Informácie o identite v Yammeri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664185"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="7d139-102">Informácie o identite v Yammeri</span><span class="sxs-lookup"><span data-stu-id="7d139-102">About identity in Yammer</span></span>

<span data-ttu-id="7d139-103">Odporúča sa, aby všetky siete vychádzali z nasledujúcich krokov, aby sa predišlo problémom s identitou:</span><span class="sxs-lookup"><span data-stu-id="7d139-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="7d139-104">Vynútenie identity balíka Office 365 po zriadení konta Microsoft 365 pre používateľov v službe Azure AD na zabezpečenie toho, aby sa všetci používatelia prihlásili pomocou svojho primárneho konta Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7d139-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="7d139-105">Ďalšie informácie nájdete v téme [vynútenie identity balíka Office 365 pre používateľov yammera](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="7d139-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="7d139-106">Zlúčenie viacerých sietí Yammera.</span><span class="sxs-lookup"><span data-stu-id="7d139-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="7d139-107">Staršie konfigurácie Yammera povoľujú pripojenie viacerých sietí siete Yammer k jednému nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="7d139-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="7d139-108">Ďalšie informácie nájdete v téme [migrácia siete – zlúčenie viacerých sietí yammera](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="7d139-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="7d139-109">Voliteľne môžete vynútiť licencie pre Yammer na blokovanie používateľov z Yammera, ak nemajú licenciu.</span><span class="sxs-lookup"><span data-stu-id="7d139-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="7d139-110">Ďalšie informácie nájdete v téme [Správa používateľských licencií yammera v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="7d139-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="7d139-111">Nakoniec auditovanie zoznamu používateľov pre staršie siete Yammer a pozastavenie starších používateľov.</span><span class="sxs-lookup"><span data-stu-id="7d139-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="7d139-112">Namiesto ich odstránenia sa odporúča pozastaviť (deaktivovať) používateľov, pretože odstránenie je nezvratné.</span><span class="sxs-lookup"><span data-stu-id="7d139-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="7d139-113">Ďalšie informácie nájdete v téme [auditovanie používateľov yammera v sieťach pripojených k Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) a [odstraňovanie používateľov](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="7d139-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="7d139-114">Konfiguráciou Yammera pomocou týchto krokov budete tiež pripravení na konfiguráciu siete Yammer pre natívny režim pre Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7d139-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="7d139-115">Ďalšie informácie nájdete v téme [Konfigurácia siete Yammer pre natívny režim pre Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="7d139-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>