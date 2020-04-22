---
title: Vytvorenie politík a profilov Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: fac2a9e41449b4eb9b87d21d4cba4f6f5192d9c6
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715411"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="c502a-102">Vytvorenie politiky a profilov Intune</span><span class="sxs-lookup"><span data-stu-id="c502a-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="c502a-103">V Intune, môžete vytvoriť politiky a profily, ktoré robia rôzne veci.</span><span class="sxs-lookup"><span data-stu-id="c502a-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="c502a-104">**Profily registrácie**: predkonfigurovaním zariadení podľa platformy, umožnite afinitu používateľa, použite viacnásobné overovanie a ďalšie.</span><span class="sxs-lookup"><span data-stu-id="c502a-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="c502a-105">[Čo je to registrácia zariadenia](https://docs.microsoft.com/intune/device-enrollment), a vytvoriť registračný profily pre [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)a [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) sú dobré zdroje.</span><span class="sxs-lookup"><span data-stu-id="c502a-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="c502a-106">**Politiky súladu**: definujte pravidlá a nastavenia, ktoré musia zariadenia dodržiavať, aby boli kompatibilné.</span><span class="sxs-lookup"><span data-stu-id="c502a-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="c502a-107">Môžete tiež použiť politiky súladu na monitorovanie zariadení a upozorniť používateľov na nesúlad.</span><span class="sxs-lookup"><span data-stu-id="c502a-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="c502a-108">Začíname pracovať so [zásadami súladu so zariadením](https://docs.microsoft.com/intune/device-compliance-get-started).</span><span class="sxs-lookup"><span data-stu-id="c502a-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="c502a-109">**Podmienky podmieneného prístupu**: zabezpečte organizačné prostriedky v závislosti od podmienok, ktoré zadáte.</span><span class="sxs-lookup"><span data-stu-id="c502a-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="c502a-110">Napríklad v prípade zariadení, ktoré nie sú kompatibilné, použite podmienený prístup na obmedzenie prístupu k e-mailu a SharePointu.</span><span class="sxs-lookup"><span data-stu-id="c502a-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="c502a-111">[Čo je podmienený prístup](https://docs.microsoft.com/intune/conditional-access) a [bežné spôsoby použitia podmieneného prístupu](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) sú dobré zdroje, aby ste mohli začať.</span><span class="sxs-lookup"><span data-stu-id="c502a-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="c502a-112">**Konfiguračné profily**: Spravujte funkcie a nastavenia v zariadeniach, vrátane nastavení e-mailu, pridania Wi-Fi siete, používania vstavaných šablón, ovládacích prvkov zariadenia iOS a macOS a ďalších funkcií.</span><span class="sxs-lookup"><span data-stu-id="c502a-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="c502a-113">Začnite v [profiloch konfigurácie zariadenia](https://docs.microsoft.com/intune/device-profiles).</span><span class="sxs-lookup"><span data-stu-id="c502a-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="c502a-114">Užitočné odkazy:</span><span class="sxs-lookup"><span data-stu-id="c502a-114">Helpful links:</span></span>

- [<span data-ttu-id="c502a-115">Bežné otázky, problémy a rozlíšenia so zásadami a profilmi zariadenia v Intune</span><span class="sxs-lookup"><span data-stu-id="c502a-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="c502a-116">Riešenie problémov s politikami a profilmi v Intune</span><span class="sxs-lookup"><span data-stu-id="c502a-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
