---
title: Používanie e-mailových profilov so službou Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653303"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="e6ddb-102">Používanie e-mailových profilov so službou Intune</span><span class="sxs-lookup"><span data-stu-id="e6ddb-102">Using email profiles with Intune</span></span>

<span data-ttu-id="e6ddb-103">Intune sa môže použiť na vytvorenie a nasadenie e-mailových profilov pre natívny (vstavaný) e-mailového klienta na viacerých platformách zariadení.</span><span class="sxs-lookup"><span data-stu-id="e6ddb-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="e6ddb-104">Informácie o niektorých obmedzeniach, ktoré sú priradené k e-mailovým profilom vrátane spôsobu spracovania prítomnosti existujúcich profilov a odstraňovania e-mailových profilov, nájdete v téme [Pridanie nastavení e-mailu do zariadení pomocou služby Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="e6ddb-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="e6ddb-105">Ďalšie informácie o tom, ako vytvoriť e-mailové profily pre každú platformu zariadenia, nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="e6ddb-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="e6ddb-106">Nastavenie zariadenia s Androidom na konfiguráciu e-mailu, overovania a synchronizácie v službe Intune</span><span class="sxs-lookup"><span data-stu-id="e6ddb-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="e6ddb-107">Pridanie nastavení e-mailu pre zariadenia so systémom iOS a iPadOS v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e6ddb-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="e6ddb-108">Nastavenie e-mailového profilu v službe Microsoft Intune pre zariadenia s operačným systémom Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="e6ddb-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="e6ddb-109">Nastavenie e-mailového profilu pre zariadenia s Windowsom 10 v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e6ddb-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="e6ddb-110">**Bežný problém so synchronizáciou**</span><span class="sxs-lookup"><span data-stu-id="e6ddb-110">**Common syncing issue**</span></span>

<span data-ttu-id="e6ddb-111">**Platforma KNOX v e-mailovom profile pre Android zabraňuje synchronizácii používateľských kontaktov, kalendára a úloh v synchronizácii s používateľskými zariadeniami.**</span><span class="sxs-lookup"><span data-stu-id="e6ddb-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="e6ddb-112">E-mailový profil KNOX v systéme Android KNOX poskytuje správcovi možnosť rozhodnúť sa, ktoré typy obsahu sa synchronizujú so zariadením, nastavením jednotlivých povolení.</span><span class="sxs-lookup"><span data-stu-id="e6ddb-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="e6ddb-113">Ak je nastavenie pre ktorýkoľvek z typov obsahu nastavené na možnosť **nie je nakonfigurované** (predvolené), daný typ obsahu sa nesynchronizuje automaticky.</span><span class="sxs-lookup"><span data-stu-id="e6ddb-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="e6ddb-114">Používateľ môže povoliť manuálne nastavenie typu obsahu priamo v zariadení, ale táto konfigurácia sa prepíše nastavením politiky služby Intune a synchronizácia sa prestane pre daný typ obsahu.</span><span class="sxs-lookup"><span data-stu-id="e6ddb-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

