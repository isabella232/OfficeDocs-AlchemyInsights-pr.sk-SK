---
title: Informácie o identite v Yammeri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148303"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="168c6-102">Informácie o identite v Yammeri</span><span class="sxs-lookup"><span data-stu-id="168c6-102">About identity in Yammer</span></span>

<span data-ttu-id="168c6-103">Odporúča sa, aby všetky siete prijali nasledujúce kroky, aby sa zabránilo otázkam súvisiacim s identitou:</span><span class="sxs-lookup"><span data-stu-id="168c6-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="168c6-104">Vynútenie identity služieb Office 365 po poskytnutí kont Microsoft 365 pre používateľov v službe Azure AD, aby ste sa uistili, že sa všetci používatelia prihlasujú pomocou primárneho konta Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="168c6-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="168c6-105">Ďalšie informácie nájdete v téme [Vynútenie identity služieb Office 365 pre používateľov yammera](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="168c6-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="168c6-106">Konsolidujte viaceré siete Yammer.</span><span class="sxs-lookup"><span data-stu-id="168c6-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="168c6-107">Staršie konfigurácie yammera umožňujú pripojenie viacerých sietí Yammer k jednému nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="168c6-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="168c6-108">Ďalšie informácie nájdete v téme [Migrácia siete – konsolidácia viacerých sietí Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="168c6-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="168c6-109">Voliteľne vynútiť licencovanie pre Yammer blokovať používateľov z Yammer, ak nemajú licenciu.</span><span class="sxs-lookup"><span data-stu-id="168c6-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="168c6-110">Ďalšie informácie nájdete v téme [Správa používateľských licencií yammera v službách Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="168c6-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="168c6-111">Nakoniec auditovať zoznam používateľov starších sietí Yammer a pozastaviť starších používateľov.</span><span class="sxs-lookup"><span data-stu-id="168c6-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="168c6-112">Odporúča sa, aby ste namiesto ich odstránenia pozastavili (deaktivovali) používateľov, pretože odstránenie je nezvratné.</span><span class="sxs-lookup"><span data-stu-id="168c6-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="168c6-113">Ďalšie informácie nájdete [v témach Auditovanie používateľov Yammera v sieťach pripojených k službám Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) a [Odstránenie používateľov](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="168c6-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="168c6-114">Konfigurácia Yammerpomocou týchto krokov, budete tiež pripravení nakonfigurovať sieť Yammer pre natívny režim pre Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="168c6-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="168c6-115">Ďalšie informácie nájdete v téme [Konfigurácia siete Yammer pre natívny režim pre microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="168c6-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>