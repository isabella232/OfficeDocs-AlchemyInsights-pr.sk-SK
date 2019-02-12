---
title: Chyba rozhrania Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903126"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="5c051-102">Chyba rozhrania Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="5c051-102">Winsock error 10061</span></span>

<span data-ttu-id="5c051-p101">Tento kód chyby znamená, že Office 365 nemohol vytvoriť soket TCP (pripojenie) s cieľového hostiteľa. Najpravdepodobnejšou príčinou vzniku tejto chyby je problém s konfiguráciou brány firewall. Ak chcete vyriešiť tento problém, skontrolujte tieto nastavenia:</span><span class="sxs-lookup"><span data-stu-id="5c051-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="5c051-106">Overte konfiguráciu brány firewall s informáciami v [Office 365 URL a IP rozsahu adries](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="5c051-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="5c051-107">Ak chyba je špecifická pre Exchange Online Protection (EOP), ste mali predtým oznámili zmenu na [Exchange Online Protection IP adries](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="5c051-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="5c051-108">Overiť, že váš Internet Service Provider (ISP) nie je blokovanie portov.</span><span class="sxs-lookup"><span data-stu-id="5c051-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="5c051-109">Overenie smart hostiteľským a cieľovým server nastavenia vo vašom konektory.</span><span class="sxs-lookup"><span data-stu-id="5c051-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="5c051-110">Všimnite si, že Office 365 nemá blokovať *prichádzajúce* pripojenia týmto spôsobom.</span><span class="sxs-lookup"><span data-stu-id="5c051-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

