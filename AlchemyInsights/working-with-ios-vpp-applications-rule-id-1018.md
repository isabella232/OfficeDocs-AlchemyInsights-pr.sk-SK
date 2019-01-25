---
title: Práca s iOS VPP aplikácie pravidla Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29488933"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="9a4f5-102">Práca s iOS VPP aplikácie</span><span class="sxs-lookup"><span data-stu-id="9a4f5-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="9a4f5-103">Čítať [ako zvládať iOS aplikácie zakúpené prostredníctvom programu objem nákupu s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) sa dozvedieť o funkcie, obmedzenia a kroky, aby sa Apple objem nákupu Program a podporu pre to v Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="9a4f5-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="9a4f5-104">**Spoločné otázky:** "IOS VPP aplikácie priradené používateľom, ale Inštalácia zlyhala."</span><span class="sxs-lookup"><span data-stu-id="9a4f5-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="9a4f5-p101">To môže nastať ak jeden token VPP sa používa vo viacerých poskytovateľov riešení na správu mobilných zariadení. VPP tokeny od Apple môže byť použité iba s jedným poskytovateľom. Ak ste použili VPP token s viacerými poskytovateľmi, musí re-upload token Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="9a4f5-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="9a4f5-p102">Inštalácia tiež môže zlyhať, ak celkový počet zariadení presiahnuť počet licencií. Zobraziť zostavy používania pre vaše licencie, prejdite na **Windows Intune mobilné aplikácie** \> stránke **aplikácie licencie** . Naučiť sa kultivovať licencií používaných, pozri [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="9a4f5-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

