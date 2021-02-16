---
title: Skupinová politika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256905"
---
# <a name="group-policy"></a><span data-ttu-id="36ed3-102">Skupinová politika</span><span class="sxs-lookup"><span data-stu-id="36ed3-102">Group policy</span></span>

<span data-ttu-id="36ed3-103">Nastavenia pre objekty používateľov a počítača v doménových službách Azure Active Directory (Azure AD DS) sa často spravujú pomocou objektov skupinovej politiky (GPO).</span><span class="sxs-lookup"><span data-stu-id="36ed3-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="36ed3-104">Azure AD DS obsahuje vstavané objekty GPO pre AADDC používateľov a kontajnery na AADDC počítače.</span><span class="sxs-lookup"><span data-stu-id="36ed3-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="36ed3-105">Tieto vstavané GPOs môžete prispôsobiť tak, aby sa Skupinová politika podľa potreby nakonfigurovala pre vaše prostredie.</span><span class="sxs-lookup"><span data-stu-id="36ed3-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="36ed3-106">Členovia skupiny Správcovia služby Azure AD DC majú oprávnenia na správu skupinovej politiky v doméne Azure AD DS a môžu tiež vytvárať vlastné GPOs a organizačné jednotky (organizačné jednotky).</span><span class="sxs-lookup"><span data-stu-id="36ed3-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="36ed3-107">Ďalšie informácie o tom, čo je Skupinová politika a ako funguje, nájdete v téme [Prehľad skupinovej politiky](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="36ed3-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="36ed3-108">V hybridnom prostredí sa skupinové politiky nakonfigurované v lokálnom prostredí AD DS nesynchronizujú so službou Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="36ed3-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="36ed3-109">Ak chcete definovať nastavenia konfigurácie pre používateľov alebo počítače v službe Azure AD DS, upravte niektorú z predvolených GPOs alebo vytvorte vlastný objekt GPO.</span><span class="sxs-lookup"><span data-stu-id="36ed3-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="36ed3-110">V tomto článku sa [spravuje Skupinová politika](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) , ktorá vám ukáže, ako nainštalovať nástroje na správu skupinovej politiky, ako Tony upraviť vstavané GPOs a ako vytvoriť vlastné GPOs.</span><span class="sxs-lookup"><span data-stu-id="36ed3-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



