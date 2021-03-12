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
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704909"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="8253d-102">Riešenie problémov s hlásením odmietnutia prístupu</span><span class="sxs-lookup"><span data-stu-id="8253d-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="8253d-103">Ak sa do zdieľaného priečinka v SharePointe zobrazila správa prístup odmietnutý, správca kolekcie lokalít mohol povoliť režim uzamknutia obmedzeného prístupu používateľa s obmedzeným prístupom.</span><span class="sxs-lookup"><span data-stu-id="8253d-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="8253d-104">Ak chcete túto funkciu vypnúť:</span><span class="sxs-lookup"><span data-stu-id="8253d-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="8253d-105">Prejdite na lokalitu, kliknite na ikonu nastavenia a potom kliknite na položku **Nastavenie lokality**.</span><span class="sxs-lookup"><span data-stu-id="8253d-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="8253d-106">V časti **Správa kolekcie lokalít** kliknite na položku **funkcie kolekcie lokalít**.</span><span class="sxs-lookup"><span data-stu-id="8253d-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="8253d-107">Vedľa **režimu uzamknutia povolenia používateľa s obmedzeným prístupom** kliknite na položku **deaktivovať**.</span><span class="sxs-lookup"><span data-stu-id="8253d-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="8253d-108">Ak je lokalita publikačnou lokalitou, môže sa stať, že správa je odmietnutý aj v prípade zdieľaných priečinkov.</span><span class="sxs-lookup"><span data-stu-id="8253d-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="8253d-109">Informácie nájdete v téme [prístup odmietnutý pri prístupe k zdieľanému priečinku](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="8253d-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="8253d-110">Ak sa pri pokuse o zobrazenie žiadostí o prístup zobrazila správa "prístup odmietnutý", používateľ sa musí pridať ako správca kolekcie lokalít alebo člen skupiny vlastníci lokality.</span><span class="sxs-lookup"><span data-stu-id="8253d-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="8253d-111">Ďalšie informácie nájdete v téme [prístup odmietnutý do zoznamu žiadosti o prístup](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="8253d-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="8253d-112">Ak sa používateľovi zobrazila správa prístup odmietnutý po odstránení z lokálnej služby Active Directory a potom sa pridal späť, prečítajte si tému [prístup odmietnutý, keď sa používateľské konto synchronizuje so službou Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="8253d-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

