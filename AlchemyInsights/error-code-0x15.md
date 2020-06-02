---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ak sa pri aktivácii balíka Office 2013 na nasadenie služieb vzdialenej pracovnej plochy (RDS) zobrazuje chyba, zvážte povolenie adalu úpravou databázy Registry.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506861"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="9177b-103">Chyba pri aktivácii balíka Office 2013 v službách vzdialenej pracovnej plochy</span><span class="sxs-lookup"><span data-stu-id="9177b-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="9177b-104">Ak sa pri aktivácii balíka Office 2013 na nasadenie služieb vzdialenej pracovnej plochy (RDS) zobrazuje chyba, zvážte povolenie adalu úpravou databázy Registry.</span><span class="sxs-lookup"><span data-stu-id="9177b-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="9177b-105">**Kľúč databázy Registry**</span><span class="sxs-lookup"><span data-stu-id="9177b-105">**Registry key**</span></span>|<span data-ttu-id="9177b-106">**Typ**</span><span class="sxs-lookup"><span data-stu-id="9177b-106">**Type**</span></span>|<span data-ttu-id="9177b-107">**Hodnota**</span><span class="sxs-lookup"><span data-stu-id="9177b-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9177b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="9177b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="9177b-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="9177b-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="9177b-110">1</span><span class="sxs-lookup"><span data-stu-id="9177b-110">1</span></span>  <br/> |

<span data-ttu-id="9177b-111">Ďalšie informácie sa nachádzajú v téme [Povolenie moderného overovania balíka Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="9177b-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="9177b-112">ADAL je predvolene zapnutá v aplikáciách Microsoft 365 pre podniky a Office 2016.</span><span class="sxs-lookup"><span data-stu-id="9177b-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="9177b-113">Služby vzdialenej pracovnej plochy (RDS) sa predtým nazývali terminálové služby.</span><span class="sxs-lookup"><span data-stu-id="9177b-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  