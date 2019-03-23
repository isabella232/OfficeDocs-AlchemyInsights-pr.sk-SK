---
title: 932 inovácia AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778756"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="08613-102">Aktualizácia Azure AD pripojenie</span><span class="sxs-lookup"><span data-stu-id="08613-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="08613-103">Podľa predvoleného nastavenia automatické aktualizácie zapnuté Azure AD pripojiť, ktorý pomáha zabezpečiť, že používate najnovšiu verziu.</span><span class="sxs-lookup"><span data-stu-id="08613-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="08613-104">Nastavenie automatického upgrade, pomocou Azure AD PowerShell cmdlet **Get-ADSyncAutoUpgrade** .</span><span class="sxs-lookup"><span data-stu-id="08613-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="08613-105">Rutiny cmdlet vráti niektorú z nasledujúcich hodnôt:</span><span class="sxs-lookup"><span data-stu-id="08613-105">The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="08613-106">**Zapnuté**: Automatické aktualizácie zapnutá.</span><span class="sxs-lookup"><span data-stu-id="08613-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="08613-107">**Vypnuté**: Automatické aktualizácie je vypnuté.</span><span class="sxs-lookup"><span data-stu-id="08613-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="08613-108">**Zavesené**: systém už nie je oprávnený prijímať automatické aktualizácie.</span><span class="sxs-lookup"><span data-stu-id="08613-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="08613-109">Nemôžete konfigurovať túto hodnotu; nachádza sa v systéme.</span><span class="sxs-lookup"><span data-stu-id="08613-109">You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="08613-110">Ďalšie informácie nájdete v [Automatické aktualizácie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="08613-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="08613-111">Stiahnuť najnovšiu verziu Azure AD pripojenie, prejdite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="08613-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

