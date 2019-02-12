---
title: Práca s iOS VPP aplikácie pravidla Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917511"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="7e84b-102">Práca s iOS VPP aplikácie</span><span class="sxs-lookup"><span data-stu-id="7e84b-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="7e84b-103">Čítať [ako zvládať iOS aplikácie zakúpené prostredníctvom programu objem nákupu s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) sa dozvedieť o funkcie, obmedzenia a kroky, aby sa Apple objem nákupu Program a podporu pre to v Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="7e84b-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="7e84b-104">**Spoločné otázky:** "IOS VPP aplikácie priradené používateľom, ale Inštalácia zlyhala."</span><span class="sxs-lookup"><span data-stu-id="7e84b-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="7e84b-p101">To môže nastať ak jeden token VPP sa používa vo viacerých poskytovateľov riešení na správu mobilných zariadení. VPP tokeny od Apple môže byť použité iba s jedným poskytovateľom. Ak ste použili VPP token s viacerými poskytovateľmi, musí re-upload token Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="7e84b-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="7e84b-p102">Inštalácia tiež môže zlyhať, ak celkový počet zariadení presiahnuť počet licencií. Zobraziť zostavy používania pre vaše licencie, prejdite na **Windows Intune mobilné aplikácie** \> stránke **aplikácie licencie** . Naučiť sa kultivovať licencií používaných, pozri [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="7e84b-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

