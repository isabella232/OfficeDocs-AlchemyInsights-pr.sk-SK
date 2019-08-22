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
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500434"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="faec2-102">Riešenie problémov so správami prístup odmietnutý</span><span class="sxs-lookup"><span data-stu-id="faec2-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="faec2-103">Ak niekto dostal hlásenie "Prístup odmietnutý" na zdieľaný priečinok v službe SharePoint, správca kolekcie lokality môže povolili "obmedzeným prístupom používateľ povolenie uzamknutie móde."</span><span class="sxs-lookup"><span data-stu-id="faec2-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="faec2-104">Vypnutie:</span><span class="sxs-lookup"><span data-stu-id="faec2-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="faec2-105">Prejdite na lokalitu, kliknite na ikonu nastavenia a potom kliknite na položku **Nastavenie lokality**.</span><span class="sxs-lookup"><span data-stu-id="faec2-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="faec2-106">V časti **Správa kolekcie lokalít**kliknite na položku **funkcie kolekcie lokality**.</span><span class="sxs-lookup"><span data-stu-id="faec2-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="faec2-107">Vedľa **obmedzeným prístupom používateľ povolenie uzamknutie režime**, kliknite na tlačidlo **deaktivovať**.</span><span class="sxs-lookup"><span data-stu-id="faec2-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="faec2-108">Hlásenie prístup odmietnutý môže tiež nastať pre zdieľané priečinky, ak lokalita publikačná lokalita.</span><span class="sxs-lookup"><span data-stu-id="faec2-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="faec2-109">Informácie nájdete v téme [Prístup odmietnutý pri prístupe k zdieľaným priečinkom](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="faec2-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="faec2-110">Ak niekto dostal hlásenie "Prístup odmietnutý" pri pokuse zobraziť žiadosť o prístup, používateľ potrebuje doplniť ako správca kolekcie lokality alebo členom skupiny vlastníci lokality.</span><span class="sxs-lookup"><span data-stu-id="faec2-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="faec2-111">Ďalšie informácie nájdete v téme [Odmietnutý prístup k zoznamu žiadostí o prístup](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="faec2-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="faec2-112">Ak používateľ dostal hlásenie "Prístup odmietnutý", potom boli odstránené z lokálnej služby Active Directory a potom pridá späť, vidieť [Prístup odmietnutý pri používateľské konto je synchronizované s Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="faec2-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

