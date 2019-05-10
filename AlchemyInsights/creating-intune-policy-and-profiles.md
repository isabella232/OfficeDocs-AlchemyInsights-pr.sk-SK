---
title: Vytvoriť Windows Intune politík a profily
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 05/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 6700005
ms.openlocfilehash: 3fecad7d02b8e3148a3dd774d666fc4ed317204c
ms.sourcegitcommit: 7e2122a7e08525f628986978f396b3a138d2326d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/07/2019
ms.locfileid: "33661749"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="3c41a-102">Vytvorenie politiky Intune a profily</span><span class="sxs-lookup"><span data-stu-id="3c41a-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="3c41a-103">V Windows Intune, môžete vytvoriť politiky a profily, ktoré robiť rôzne veci.</span><span class="sxs-lookup"><span data-stu-id="3c41a-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="3c41a-104">**Registrácia profilov**: vopred nakonfigurovať zariadenia platformy, umožňujú užívateľovi afinitu, použite viacnásobné overovanie, a ďalšie.</span><span class="sxs-lookup"><span data-stu-id="3c41a-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span> 

  <span data-ttu-id="3c41a-105">[Čo je registrácia zariadení](https://docs.microsoft.com/intune/device-enrollment), vytvoriť zápis profily pre [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)a [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) sú dobré zdroje.</span><span class="sxs-lookup"><span data-stu-id="3c41a-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="3c41a-106">**Súlad politík**: definovať pravidlá a nastavenia, ktoré zariadenia musia dodržiavať v súlade.</span><span class="sxs-lookup"><span data-stu-id="3c41a-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="3c41a-107">Môžete tiež použiť súladu politiky monitorovať zariadenia a informovať používateľov o nesúlad.</span><span class="sxs-lookup"><span data-stu-id="3c41a-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span> 

  <span data-ttu-id="3c41a-108">Začíname používať [zariadenie súladu politiky](https://docs.microsoft.com/intune/device-compliance-get-started).</span><span class="sxs-lookup"><span data-stu-id="3c41a-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="3c41a-109">**Podmieneného prístupu politiky**: pomôcť zabezpečené organizačné zdroje, v závislosti od podmienok, ktoré zadáte.</span><span class="sxs-lookup"><span data-stu-id="3c41a-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="3c41a-110">Napríklad pre zariadenia, ktoré nie sú kompatibilné s, pomocou podmieneného prístupu obmedziť prístup k e-mailu a SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3c41a-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="3c41a-111">[Čo je podmienený prístup](https://docs.microsoft.com/intune/conditional-access) a [bežné spôsoby používania podmieneného prístupu](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) sú dobré zdroje začať.</span><span class="sxs-lookup"><span data-stu-id="3c41a-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="3c41a-112">**Konfigurácia profily**: spravovanie funkcií a nastavení na zariadeniach, vrátane nastavenia e-mailu, pridať sieť Wi-Fi, použite vstavaný šablóny a ovládanie funkcií zariadenia iOS a macOS.</span><span class="sxs-lookup"><span data-stu-id="3c41a-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span> 

  <span data-ttu-id="3c41a-113">Začíname v [zariadení konfiguračných profilov](https://docs.microsoft.com/intune/device-profiles).</span><span class="sxs-lookup"><span data-stu-id="3c41a-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="3c41a-114">Užitočné odkazy:</span><span class="sxs-lookup"><span data-stu-id="3c41a-114">Helpful links:</span></span>

- [<span data-ttu-id="3c41a-115">Spoločné otázky, problémy a rezolúcií s politiky zariadení a profily vo Windows Intune</span><span class="sxs-lookup"><span data-stu-id="3c41a-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="3c41a-116">Riešenie problémov s politikami a profily vo Windows Intune</span><span class="sxs-lookup"><span data-stu-id="3c41a-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
