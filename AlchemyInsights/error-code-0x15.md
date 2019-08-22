---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527061"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="54dfa-103">Chyba pri aktivácii Office 2013 na služby vzdialenej pracovnej plochy</span><span class="sxs-lookup"><span data-stu-id="54dfa-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="54dfa-104">Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.</span><span class="sxs-lookup"><span data-stu-id="54dfa-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="54dfa-105">**Kľúč databázy Registry**</span><span class="sxs-lookup"><span data-stu-id="54dfa-105">**Registry key**</span></span>|<span data-ttu-id="54dfa-106">**Typ**</span><span class="sxs-lookup"><span data-stu-id="54dfa-106">**Type**</span></span>|<span data-ttu-id="54dfa-107">**Hodnota**</span><span class="sxs-lookup"><span data-stu-id="54dfa-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="54dfa-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="54dfa-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="54dfa-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="54dfa-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="54dfa-110">1</span><span class="sxs-lookup"><span data-stu-id="54dfa-110">1</span></span>  <br/> |

<span data-ttu-id="54dfa-111">Ďalšie informácie, pozrite si [Umožňujú moderné overenie Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="54dfa-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="54dfa-112">ADAL zapnutá v predvolenom nastavení Office 365 ProPlus a Office 2016.</span><span class="sxs-lookup"><span data-stu-id="54dfa-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="54dfa-113">Remote Desktop Services (RDS) bol predtým pomenovaný terminálových služieb.</span><span class="sxs-lookup"><span data-stu-id="54dfa-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  