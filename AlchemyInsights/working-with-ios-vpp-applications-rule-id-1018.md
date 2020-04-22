---
title: Práca s iOS VPP aplikácie ID pravidla 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719972"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="a3afd-102">Práca s aplikáciami systému iOS VPP</span><span class="sxs-lookup"><span data-stu-id="a3afd-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="a3afd-103">Prečítajte si, [ako spravovať aplikácie pre iOS zakúpené prostredníctvom programu na nákup zväzku s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) a dozvedieť sa o funkciách, obmedzeniach a krokoch, aby ste mohli využiť program na nákup zväzku Apple a podporu pre ňu v Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a3afd-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="a3afd-104">**Bežné problémy:** "Priradil som aplikáciu iOS VPP k mojim používateľom, ale Inštalácia zlyhala."</span><span class="sxs-lookup"><span data-stu-id="a3afd-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="a3afd-105">Môže sa to stať, ak sa v rámci viacerých poskytovateľov správy mobilných zariadení používa jediný token VPP.</span><span class="sxs-lookup"><span data-stu-id="a3afd-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="a3afd-106">Žetóny VPP od spoločnosti Apple sa môžu používať iba s jedným poskytovateľom.</span><span class="sxs-lookup"><span data-stu-id="a3afd-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="a3afd-107">Ak ste použili token VPP s viacerými poskytovateľmi, musíte znova odovzdať token Intune.</span><span class="sxs-lookup"><span data-stu-id="a3afd-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="a3afd-108">Inštalácia môže zlyhať aj v prípade, že celkový počet inštalácií prekročí počet licencií.</span><span class="sxs-lookup"><span data-stu-id="a3afd-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="a3afd-109">Ak chcete zobraziť zostavu používania pre svoje licencie, prejdite na stránku **licencie aplikácie** **Intune Mobile Apps** \> .</span><span class="sxs-lookup"><span data-stu-id="a3afd-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="a3afd-110">Ďalšie informácie o možnostiach opätovného použitia licencií nájdete v [tomto článku.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="a3afd-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
