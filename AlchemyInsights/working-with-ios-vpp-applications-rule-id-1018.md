---
title: Práca so systémom iOS aplikácie VPP Applications ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688961"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="10ffa-102">Práca s aplikáciami VPP v systéme iOS</span><span class="sxs-lookup"><span data-stu-id="10ffa-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="10ffa-103">Prečítajte si, [ako spravovať aplikácie systému iOS zakúpené prostredníctvom programu na hromadné](https://docs.microsoft.com/intune/vpp-apps-ios) zakúpenie v službe Microsoft Intune, kde získate informácie o funkciách, obmedzeniach a krokoch, ktoré vám pomôžu využiť program na nákup zväzkov Apple a podporu pre IT v službe Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="10ffa-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="10ffa-104">**Bežné problémy:** "Priradenú aplikáciu VPP pre systém iOS pre používateľov, ale Inštalácia zlyhala."</span><span class="sxs-lookup"><span data-stu-id="10ffa-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="10ffa-105">Môže sa to stať, ak sa v rámci viacerých poskytovateľov správy mobilných zariadení používa jeden token VPP.</span><span class="sxs-lookup"><span data-stu-id="10ffa-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="10ffa-106">Tokeny VPP od spoločnosti Apple sa môžu používať len s jedným poskytovateľom.</span><span class="sxs-lookup"><span data-stu-id="10ffa-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="10ffa-107">Ak ste použili token VPP s viacerými poskytovateľmi, token sa musí znova nahrať do služby Intune.</span><span class="sxs-lookup"><span data-stu-id="10ffa-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="10ffa-108">Inštalácia môže zlyhať aj v prípade, ak celkový počet inštalácií prekročí počet licencií.</span><span class="sxs-lookup"><span data-stu-id="10ffa-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="10ffa-109">Ak chcete zobraziť zostavu používania pre svoje licencie, prejdite na stránku licencie aplikácií pre **mobilné aplikácie Intune** \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="10ffa-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="10ffa-110">Ak sa chcete dozvedieť, ako sa pri používaní licencií uplatniť, prečítajte si [Tento článok.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="10ffa-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
