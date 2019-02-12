---
title: Riešenie problémov so správami prístup odmietnutý
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f1a4803838b6511ef4fe7f03cafa4aa13b3c9734
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916467"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="b0a55-102">Riešenie problémov so správami prístup odmietnutý</span><span class="sxs-lookup"><span data-stu-id="b0a55-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="b0a55-p101">Ak niekto dostal hlásenie "Prístup odmietnutý" do zdieľaného priečinka, správca kolekcie lokality môže povolili "obmedzeným prístupom používateľ povolenie uzamknutie móde." Vypnutie:</span><span class="sxs-lookup"><span data-stu-id="b0a55-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="b0a55-105">Prejdite na lokalitu, kliknite na ikonu nastavenia a potom kliknite na položku **Nastavenie lokality**.</span><span class="sxs-lookup"><span data-stu-id="b0a55-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="b0a55-106">V časti **Správa kolekcie lokalít**kliknite na položku **funkcie kolekcie lokality**.</span><span class="sxs-lookup"><span data-stu-id="b0a55-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="b0a55-107">Vedľa **obmedzeným prístupom používateľ povolenie uzamknutie režime**, kliknite na tlačidlo **deaktivovať**.</span><span class="sxs-lookup"><span data-stu-id="b0a55-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="b0a55-p102">Hlásenie prístup odmietnutý môže tiež nastať pre zdieľané priečinky, ak lokalita publikačná lokalita. Informácie nájdete v téme [Prístup odmietnutý pri prístupe k zdieľaným priečinkom](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="b0a55-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="b0a55-p103">Ak niekto dostal hlásenie "Prístup odmietnutý" pri pokuse zobraziť žiadosť o prístup, používateľ potrebuje doplniť ako správca kolekcie lokality alebo členom skupiny vlastníci lokality. Ďalšie informácie nájdete v téme [Odmietnutý prístup k zoznamu žiadostí o prístup](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="b0a55-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="b0a55-112">Ak používateľ dostal hlásenie "Prístup odmietnutý", potom boli odstránené z lokálnej služby Active Directory a potom pridá späť, vidieť [Prístup odmietnutý pri používateľské konto je synchronizované s Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="b0a55-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

