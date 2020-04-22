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
description: Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na nasadenie služby vzdialenej skúsenosti s prácou s počítačom (RDS), zvážte povolenie ADAL úpravou databázy Registry.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703153"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="1d5dc-103">Chyba pri aktivácii balíka Office 2013 služby vzdialenej skúsenosti s prácou s počítačom</span><span class="sxs-lookup"><span data-stu-id="1d5dc-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="1d5dc-104">Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na nasadenie služby vzdialenej skúsenosti s prácou s počítačom (RDS), zvážte povolenie ADAL úpravou databázy Registry.</span><span class="sxs-lookup"><span data-stu-id="1d5dc-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="1d5dc-105">**Kľúč databázy Registry**</span><span class="sxs-lookup"><span data-stu-id="1d5dc-105">**Registry key**</span></span>|<span data-ttu-id="1d5dc-106">**Typ**</span><span class="sxs-lookup"><span data-stu-id="1d5dc-106">**Type**</span></span>|<span data-ttu-id="1d5dc-107">**Hodnota**</span><span class="sxs-lookup"><span data-stu-id="1d5dc-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1d5dc-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="1d5dc-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="1d5dc-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="1d5dc-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="1d5dc-110">1</span><span class="sxs-lookup"><span data-stu-id="1d5dc-110">1</span></span>  <br/> |

<span data-ttu-id="1d5dc-111">Ďalšie informácie nájdete v časti [povolenie moderného overovania pre balík Office 2013 v zariadeniach so systémom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="1d5dc-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="1d5dc-112">ADAL je predvolene zapnutá v Microsoft 365 aplikácie pre podniky a Office 2016.</span><span class="sxs-lookup"><span data-stu-id="1d5dc-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="1d5dc-113">Služby vzdialenej pracovnej plochy (RDS) sa predtým pomenovali terminálové služby.</span><span class="sxs-lookup"><span data-stu-id="1d5dc-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  