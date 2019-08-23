---
title: Práca s iOS VPP aplikácie pravidla Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558020"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="1e342-102">Práca s iOS VPP aplikácie</span><span class="sxs-lookup"><span data-stu-id="1e342-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="1e342-103">Čítať [ako zvládať iOS aplikácie zakúpené prostredníctvom programu objem nákupu s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) sa dozvedieť o funkcie, obmedzenia a kroky, aby sa Apple objem nákupu Program a podporu pre to v Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="1e342-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="1e342-104">**Spoločné otázky:** "IOS VPP aplikácie priradené používateľom, ale Inštalácia zlyhala."</span><span class="sxs-lookup"><span data-stu-id="1e342-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="1e342-105">To môže nastať ak jeden token VPP sa používa vo viacerých poskytovateľov riešení na správu mobilných zariadení.</span><span class="sxs-lookup"><span data-stu-id="1e342-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="1e342-106">VPP tokeny od Apple môže byť použité iba s jedným poskytovateľom.</span><span class="sxs-lookup"><span data-stu-id="1e342-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="1e342-107">Ak ste použili VPP token s viacerými poskytovateľmi, musí re-upload token Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="1e342-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="1e342-108">Inštalácia tiež môže zlyhať, ak celkový počet zariadení presiahnuť počet licencií.</span><span class="sxs-lookup"><span data-stu-id="1e342-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="1e342-109">Zobraziť zostavy používania pre vaše licencie, prejdite na **Windows Intune mobilné aplikácie** \> stránke **aplikácie licencie** .</span><span class="sxs-lookup"><span data-stu-id="1e342-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="1e342-110">Naučiť sa kultivovať licencií používaných, pozri [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="1e342-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
