---
title: Používanie e-mailových profilov s intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555762"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="cd4f3-102">Používanie e-mailových profilov s intune</span><span class="sxs-lookup"><span data-stu-id="cd4f3-102">Using email profiles with Intune</span></span>

<span data-ttu-id="cd4f3-103">Intune možno vytvoriť a nasadiť e-mailové profily pre natívne (vstavaný) e-mailový klient na viacerých platformách zariadení.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="cd4f3-104">Informácie o niektorých obmedzeniach súvisiacich s e-mailovými profilmi vrátane spôsobu spracovania prítomnosti existujúcich profilov a spôsobu odstránenie e-mailových profilov nájdete v téme [Pridanie nastavení e-mailu do zariadení pomocou aplikácie Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="cd4f3-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="cd4f3-105">Ďalšie informácie o vytváraní e-mailových profilov pre každú platformu zariadení nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="cd4f3-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="cd4f3-106">Nastavenia zariadenia s Androidom na konfiguráciu e-mailov, overovania a synchronizácie v programe Intune</span><span class="sxs-lookup"><span data-stu-id="cd4f3-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="cd4f3-107">Pridanie nastavení e-mailu pre zariadenia so systémom iOS a iPadOS v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="cd4f3-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="cd4f3-108">Nastavenia e-mailového profilu v službe Microsoft Intune pre zariadenia so systémom Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="cd4f3-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="cd4f3-109">Nastavenie e-mailového profilu pre zariadenia so systémom Windows 10 v microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="cd4f3-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="cd4f3-110">**Bežný problém so synchronizáciou**</span><span class="sxs-lookup"><span data-stu-id="cd4f3-110">**Common syncing issue**</span></span>

<span data-ttu-id="cd4f3-111">**Knox v e-mailovom profile Androidu zabraňuje synchronizácii kontaktov, kalendára a úloh používateľa s používateľskými zariadeniami.**</span><span class="sxs-lookup"><span data-stu-id="cd4f3-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="cd4f3-112">E-mailový profil KNOX v systéme Android KNOX ponúka správcovi možnosť rozhodnúť sa, ktoré typy obsahu sa synchronizujú so zariadením, nastavením každého na povolené.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="cd4f3-113">Ak je nastavenie pre niektorý z typov obsahu nastavené na možnosť **Nie je nakonfigurované** (predvolené), tento typ obsahu sa nesynchronizuje automaticky.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="cd4f3-114">Používateľ môže zapnúť typ obsahu, ktorý chcete priamo v zariadení manuálne, ale táto konfigurácia sa prepíše nastavením politiky Intune a synchronizácia sa zastaví pre tento typ obsahu.</span><span class="sxs-lookup"><span data-stu-id="cd4f3-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

