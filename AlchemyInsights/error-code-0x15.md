---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ak sa zobrazuje chyba pri aktivácii služieb Office 2013 v rámci nasadenia služby Remote Desktop Services (RDS), zvážte možnosť povoliť ADAL úpravou databázy Registry.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709202"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="ec303-103">Chyba pri aktivácii služieb Office 2013 v službách vzdialenej pracovnej plochy</span><span class="sxs-lookup"><span data-stu-id="ec303-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="ec303-104">Ak sa zobrazuje chyba pri aktivácii služieb Office 2013 v rámci nasadenia služby Remote Desktop Services (RDS), zvážte možnosť povoliť ADAL úpravou databázy Registry.</span><span class="sxs-lookup"><span data-stu-id="ec303-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="ec303-105">**Kľúč databázy Registry**</span><span class="sxs-lookup"><span data-stu-id="ec303-105">**Registry key**</span></span>|<span data-ttu-id="ec303-106">**Zadajte**</span><span class="sxs-lookup"><span data-stu-id="ec303-106">**Type**</span></span>|<span data-ttu-id="ec303-107">**Hodnotu**</span><span class="sxs-lookup"><span data-stu-id="ec303-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ec303-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="ec303-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="ec303-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="ec303-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="ec303-110">1</span><span class="sxs-lookup"><span data-stu-id="ec303-110">1</span></span>  <br/> |

<span data-ttu-id="ec303-111">Ďalšie informácie nájdete v téme [povolenie moderného overovania pre Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="ec303-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="ec303-112">Funkcia ADAL je predvolene povolená v aplikáciách Microsoft 365 pre podniky a Office 2016.</span><span class="sxs-lookup"><span data-stu-id="ec303-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="ec303-113">Služby Remote Desktop Services (RDS) sa predtým nazývali terminálové služby.</span><span class="sxs-lookup"><span data-stu-id="ec303-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  