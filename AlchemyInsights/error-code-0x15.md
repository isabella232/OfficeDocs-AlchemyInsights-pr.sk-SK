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
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388260"
---
<span data-ttu-id="288c8-103">Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.</span><span class="sxs-lookup"><span data-stu-id="288c8-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="288c8-104">**Kľúč databázy Registry**</span><span class="sxs-lookup"><span data-stu-id="288c8-104">**Registry key**</span></span>|<span data-ttu-id="288c8-105">**Typ**</span><span class="sxs-lookup"><span data-stu-id="288c8-105">**Type**</span></span>|<span data-ttu-id="288c8-106">**Hodnota**</span><span class="sxs-lookup"><span data-stu-id="288c8-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="288c8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="288c8-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="288c8-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="288c8-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="288c8-109">1</span><span class="sxs-lookup"><span data-stu-id="288c8-109">1</span></span>  <br/> |

<span data-ttu-id="288c8-110">Ďalšie informácie, pozrite si [Umožňujú moderné overenie Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="288c8-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="288c8-111">ADAL zapnutá v predvolenom nastavení Office 365 ProPlus a Office 2016.</span><span class="sxs-lookup"><span data-stu-id="288c8-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="288c8-112">> remote Desktop Services (RDS) bol predtým pomenovaný terminálových služieb.</span><span class="sxs-lookup"><span data-stu-id="288c8-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  