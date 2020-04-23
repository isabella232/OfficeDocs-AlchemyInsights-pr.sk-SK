---
title: Riešenie problémov s odmietané správy programu Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759815"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="0a408-102">Riešenie problémov s odmietané správy programu Access</span><span class="sxs-lookup"><span data-stu-id="0a408-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="0a408-103">Ak niekto dostal správu "prístup odmietnutý" do zdieľaného priečinka v službe SharePoint, správca kolekcie lokalít môže mať povolené "obmedzený prístup používateľa Lockdown Mode."</span><span class="sxs-lookup"><span data-stu-id="0a408-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="0a408-104">Ak chcete túto možnosť vypnúť:</span><span class="sxs-lookup"><span data-stu-id="0a408-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="0a408-105">Prejdite na lokalitu, kliknite na ikonu nastavenia a potom kliknite na položku **Nastavenie lokality**.</span><span class="sxs-lookup"><span data-stu-id="0a408-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="0a408-106">V časti **Správa kolekcie lokalít**kliknite na položku **funkcie kolekcie lokalít**.</span><span class="sxs-lookup"><span data-stu-id="0a408-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="0a408-107">Vedľa položky **režim uzamknutia povolenia používateľa s obmedzeným prístupom**kliknite na položku **deaktivovať**.</span><span class="sxs-lookup"><span data-stu-id="0a408-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="0a408-108">Správa o odmietnutí prístupu môže nastať aj pre zdieľané priečinky, ak je lokalita publikačná lokalita.</span><span class="sxs-lookup"><span data-stu-id="0a408-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="0a408-109">Informácie nájdete v téme [prístup odmietnutý pri prístupe k zdieľanému priečinku](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="0a408-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="0a408-110">Ak niekto dostal "prístup odmietnutý" hlásenie pri pokuse o zobrazenie žiadostí o prístup, používateľ musí byť pridaný buď správca kolekcie lokalít alebo člen skupiny vlastníkov lokality.</span><span class="sxs-lookup"><span data-stu-id="0a408-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="0a408-111">Ďalšie informácie nájdete v téme [prístup odmietnutý prístup zoznam požiadaviek](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="0a408-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="0a408-112">Ak používateľ dostal "prístup odmietnutý" správa po boli odstránené z Active Directory lokálne a potom sa vrátil, pozri [prístup odmietnutý, keď používateľské konto je synchronizovaný Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="0a408-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

