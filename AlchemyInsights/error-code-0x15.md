---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929105"
---
<span data-ttu-id="b1625-103">Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.</span><span class="sxs-lookup"><span data-stu-id="b1625-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="b1625-104">**Kľúč databázy Registry**</span><span class="sxs-lookup"><span data-stu-id="b1625-104">**Registry key**</span></span>|<span data-ttu-id="b1625-105">**Zadajte výraz**</span><span class="sxs-lookup"><span data-stu-id="b1625-105">**Type**</span></span>|<span data-ttu-id="b1625-106">**Hodnota**</span><span class="sxs-lookup"><span data-stu-id="b1625-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b1625-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="b1625-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="b1625-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="b1625-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="b1625-109">1</span><span class="sxs-lookup"><span data-stu-id="b1625-109">1</span></span>  <br/> |
   
<span data-ttu-id="b1625-110">Ďalšie informácie, pozrite si [Umožňujú moderné overenie Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b1625-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="b1625-p101">ADAL zapnutá v predvolenom nastavení Office 365 ProPlus a Office 2016. > remote Desktop Services (RDS) bol predtým pomenovaný terminálových služieb.</span><span class="sxs-lookup"><span data-stu-id="b1625-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

