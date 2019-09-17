---
title: Odosielanie vlastných upozornení pomocou Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992327"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="2b8c1-102">Ako posielať vlastné oznámenia používateľom spravovaných iOS a Android zariadenia</span><span class="sxs-lookup"><span data-stu-id="2b8c1-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="2b8c1-103">Vlastné upozornenia pre Intune spracováva aplikácia portálu spoločnosti v zariadení používateľa.</span><span class="sxs-lookup"><span data-stu-id="2b8c1-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="2b8c1-104">Aplikácia potom vytvorí oznámenie push na tomto zariadení.</span><span class="sxs-lookup"><span data-stu-id="2b8c1-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="2b8c1-105">Nižšie sú uvedené predpoklady zariadenia na podporu prijímania vlastných upozornení a pre aplikáciu na vytvorenie oznámenia push:</span><span class="sxs-lookup"><span data-stu-id="2b8c1-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="2b8c1-106">Zariadenie musí mať nainštalovanú aplikáciu portálu spoločnosti.</span><span class="sxs-lookup"><span data-stu-id="2b8c1-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="2b8c1-107">Zariadenie musí povoliť aplikácii portálu spoločnosti odosielať oznámenia push.</span><span class="sxs-lookup"><span data-stu-id="2b8c1-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="2b8c1-108">Keď je aplikácia nainštalovaná alebo aktualizovaná, vyzve používateľa na povolenie upozornení.</span><span class="sxs-lookup"><span data-stu-id="2b8c1-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="2b8c1-109">Zariadenia so systémom Android musia mať nainštalované služby Google Play.</span><span class="sxs-lookup"><span data-stu-id="2b8c1-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="2b8c1-110">Zariadenie musí byť zapísané s Intune.</span><span class="sxs-lookup"><span data-stu-id="2b8c1-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="2b8c1-111">Ďalšie informácie vrátane spôsobu odoslania správy nájdete v [dokumentácii k funkcii](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="2b8c1-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
