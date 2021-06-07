---
title: Konfigurácia Microsoft Intune zabezpečenia pomocou pôvodných Windows 10 zabezpečenia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794132"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="57581-102">Konfigurácia Microsoft Intune zabezpečenia pomocou pôvodných Windows 10 zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="57581-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="57581-103">Základné hodnoty zabezpečenia služby Intune pomáhajú chrániť používateľov a zariadenia.</span><span class="sxs-lookup"><span data-stu-id="57581-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="57581-104">Pôvodné hodnoty zabezpečenia Windows predkonfigurované skupiny používané na použitie známej skupiny nastavení a predvolených hodnôt odporúčaných príslušnými tímami zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="57581-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="57581-105">Vytvorením profilu pôvodného plánu zabezpečenia v programe Intune vytvoríte šablónu, ktorá sa skladá z viacerých profilov konfigurácie zariadení.</span><span class="sxs-lookup"><span data-stu-id="57581-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="57581-106">Keď nasadzujete pôvodné hodnoty zabezpečenia skupinám používateľov alebo zariadení, nastavenia sa použijú na zariadenia, ktoré sú Windows 10 novšej verzie.</span><span class="sxs-lookup"><span data-stu-id="57581-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="57581-107">Pôvodný plán zabezpečenia správy mobilných zariadení Microsoft (MDM) napríklad automaticky zapne šifrovanie BitLocker vymeniteľné jednotky, vyžaduje heslo na odomknutie zariadenia a vypne základné overovanie.</span><span class="sxs-lookup"><span data-stu-id="57581-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="57581-108">Ak predvolená hodnota vo vašom prostredí nefunguje, môžete prispôsobiť pôvodný plán a použiť potrebné nastavenia.</span><span class="sxs-lookup"><span data-stu-id="57581-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="57581-109">Pôvodné hodnoty zabezpečenia tiež pomáhajú vytvoriť end-to-end secure workflow v Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="57581-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="57581-110">Základná hodnota zabezpečenia obsahuje osvedčené postupy a odporúčania pre nastavenia, ktoré majú vplyv na zabezpečenie.</span><span class="sxs-lookup"><span data-stu-id="57581-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="57581-111">Partneri Intune s tímom zabezpečenia Windows, ktorý vytvára pôvodné hodnoty pre skupinové politiky, takže tieto odporúčania vychádzajú z rozsiahlych pokynov a rozsiahlej skúsenosti.</span><span class="sxs-lookup"><span data-stu-id="57581-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="57581-112">Ak so služby Intune iba začínate a nie ste si istí, kde začať, základné hodnoty zabezpečenia vám pomôžu rýchlo vytvoriť a nasadiť zabezpečený profil.</span><span class="sxs-lookup"><span data-stu-id="57581-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="57581-113">Ak momentálne používate skupinovú politiku, migrácia do služby Intune na účely správy je s pôvodnými plánmi zabezpečenia omnoho jednoduchšia, pretože sú zabudované do služby Intune a zahŕňajú špičkové možnosti správy.</span><span class="sxs-lookup"><span data-stu-id="57581-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="57581-114">Ďalšie informácie nájdete v téme Windows [zabezpečenia a správa](/windows/security/threat-protection/windows-security-baselines) [mobilných zariadení.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="57581-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

