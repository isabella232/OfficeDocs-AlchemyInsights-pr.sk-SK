---
title: Odoslanie vlastných oznámení so službou Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720661"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="8f1ab-102">Odoslanie vlastných oznámení používateľom spravovaných zariadení so systémom iOS a Android</span><span class="sxs-lookup"><span data-stu-id="8f1ab-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="8f1ab-103">Vlastné oznámenia pre služby Intune sú spracované v aplikácii Company Portal v zariadení používateľa.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="8f1ab-104">Aplikácia potom vytvorí oznámenie o vyžiadaní v danom zariadení.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="8f1ab-105">Nižšie sú uvedené požiadavky zariadenia, ktoré podporujú prijímanie vlastných oznámení, a v aplikácii potom vytvorte Push Oznámenie:</span><span class="sxs-lookup"><span data-stu-id="8f1ab-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="8f1ab-106">Zariadenie musí mať nainštalovanú aplikáciu firemný portál.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="8f1ab-107">Zariadenie musí povoliť, aby aplikácia spoločnosti Portal odoslala oznámenia push.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="8f1ab-108">Pri inštalácii alebo aktualizácii aplikácie sa používateľovi zobrazí výzva na povolenie oznámení.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="8f1ab-109">Zariadenia s Androidom musia mať nainštalované služby Google Play.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="8f1ab-110">Zariadenie musí byť zaregistrované v službe Intune.</span><span class="sxs-lookup"><span data-stu-id="8f1ab-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="8f1ab-111">Ďalšie informácie vrátane spôsobu odoslania správy nájdete v [dokumentácii k funkciám](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="8f1ab-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
