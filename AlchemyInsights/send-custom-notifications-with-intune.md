---
title: Odosielanie vlastných upozornení pomocou Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886872"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="c3861-102">Ako posielať vlastné oznámenia používateľom spravovaných iOS a Android zariadenia</span><span class="sxs-lookup"><span data-stu-id="c3861-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="c3861-103">Vlastné upozornenia pre Intune spracováva aplikácia portálu spoločnosti v zariadení používateľa.</span><span class="sxs-lookup"><span data-stu-id="c3861-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="c3861-104">Aplikácia potom vytvorí oznámenie push na tomto zariadení.</span><span class="sxs-lookup"><span data-stu-id="c3861-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="c3861-105">Nižšie sú uvedené predpoklady zariadenia na podporu prijímania vlastných upozornení a pre aplikáciu na vytvorenie oznámenia push:</span><span class="sxs-lookup"><span data-stu-id="c3861-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="c3861-106">Zariadenie musí mať nainštalovanú aplikáciu portálu spoločnosti.</span><span class="sxs-lookup"><span data-stu-id="c3861-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="c3861-107">Zariadenie musí povoliť aplikácii portálu spoločnosti odosielať oznámenia push.</span><span class="sxs-lookup"><span data-stu-id="c3861-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="c3861-108">Keď je aplikácia nainštalovaná alebo aktualizovaná, vyzve používateľa na povolenie upozornení.</span><span class="sxs-lookup"><span data-stu-id="c3861-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="c3861-109">Zariadenia so systémom Android musia mať nainštalované služby Google Play.</span><span class="sxs-lookup"><span data-stu-id="c3861-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="c3861-110">Zariadenie musí byť zapísané s Intune.</span><span class="sxs-lookup"><span data-stu-id="c3861-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="c3861-111">Ďalšie informácie vrátane spôsobu odoslania správy nájdete v [dokumentácii k funkcii](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="c3861-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
