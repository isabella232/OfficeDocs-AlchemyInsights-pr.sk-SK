---
title: Riešenie problémov s hlásením odmietnutia prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690798"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="ba45a-102">Riešenie problémov s hlásením odmietnutia prístupu</span><span class="sxs-lookup"><span data-stu-id="ba45a-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="ba45a-103">Ak sa do zdieľaného priečinka v SharePointe zobrazila správa prístup odmietnutý, správca kolekcie lokalít mohol povoliť režim uzamknutia obmedzeného prístupu používateľa s obmedzeným prístupom.</span><span class="sxs-lookup"><span data-stu-id="ba45a-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="ba45a-104">Ak chcete túto funkciu vypnúť:</span><span class="sxs-lookup"><span data-stu-id="ba45a-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="ba45a-105">Prejdite na lokalitu, kliknite na ikonu nastavenia a potom kliknite na položku **Nastavenie lokality**.</span><span class="sxs-lookup"><span data-stu-id="ba45a-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="ba45a-106">V časti **Správa kolekcie lokalít**kliknite na položku **funkcie kolekcie lokalít**.</span><span class="sxs-lookup"><span data-stu-id="ba45a-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="ba45a-107">Vedľa **režimu uzamknutia povolenia používateľa s obmedzeným prístupom**kliknite na položku **deaktivovať**.</span><span class="sxs-lookup"><span data-stu-id="ba45a-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="ba45a-108">Ak je lokalita publikačnou lokalitou, môže sa stať, že správa je odmietnutý aj v prípade zdieľaných priečinkov.</span><span class="sxs-lookup"><span data-stu-id="ba45a-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="ba45a-109">Informácie nájdete v téme [prístup odmietnutý pri prístupe k zdieľanému priečinku](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="ba45a-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="ba45a-110">Ak sa pri pokuse o zobrazenie žiadostí o prístup zobrazila správa "prístup odmietnutý", používateľ sa musí pridať ako správca kolekcie lokalít alebo člen skupiny vlastníci lokality.</span><span class="sxs-lookup"><span data-stu-id="ba45a-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="ba45a-111">Ďalšie informácie nájdete v téme [prístup odmietnutý do zoznamu žiadosti o prístup](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="ba45a-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="ba45a-112">Ak sa používateľovi zobrazila správa prístup odmietnutý po odstránení z lokálnej služby Active Directory a potom sa pridal späť, prečítajte si tému [prístup odmietnutý, keď sa používateľské konto synchronizuje so službou Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="ba45a-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

