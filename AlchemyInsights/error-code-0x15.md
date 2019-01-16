---
title: Kód chyby 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311204"
---
<span data-ttu-id="01fd1-103">Ak sa zobrazí chyba pri aktivácii balíka Office 2013 na Remote Desktop Services (RDS) nasadenie, zvážte možnosť zapnutia ADAL úpravou databázy registry.</span><span class="sxs-lookup"><span data-stu-id="01fd1-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="01fd1-104">**Kľúč databázy Registry**</span><span class="sxs-lookup"><span data-stu-id="01fd1-104">**Registry key**</span></span>|<span data-ttu-id="01fd1-105">**Zadajte výraz**</span><span class="sxs-lookup"><span data-stu-id="01fd1-105">**Type**</span></span>|<span data-ttu-id="01fd1-106">**Hodnota**</span><span class="sxs-lookup"><span data-stu-id="01fd1-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="01fd1-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="01fd1-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="01fd1-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="01fd1-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="01fd1-109">1</span><span class="sxs-lookup"><span data-stu-id="01fd1-109">1</span></span>  <br/> |
   
<span data-ttu-id="01fd1-110">Ďalšie informácie, pozrite si [Umožňujú moderné overenie Office 2013 v zariadeniach s Windowsom](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="01fd1-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="01fd1-p101">ADAL zapnutá v predvolenom nastavení Office 365 ProPlus a Office 2016. > Remote Desktop Services (RDS) bol predtým pomenovaný terminálových služieb.</span><span class="sxs-lookup"><span data-stu-id="01fd1-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

