---
title: Použitie pôvodných plánov zabezpečenia služby Microsoft Intune na konfiguráciu zariadení s Windowsom 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696381"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="488d9-102">Použitie základných čiar zabezpečenia služby Microsoft Intune na konfigurovanie zariadení s Windowsom 10</span><span class="sxs-lookup"><span data-stu-id="488d9-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="488d9-103">Základné údaje zabezpečenia služby Intune pomáhajú chrániť používateľov a zariadenia.</span><span class="sxs-lookup"><span data-stu-id="488d9-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="488d9-104">Základné údaje zabezpečenia sú predkonfigurované skupiny nastavení Windowsu, ktoré sa používajú na použitie známej skupiny nastavení a predvolených hodnôt odporúčaných príslušnými tímami zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="488d9-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="488d9-105">Vytvorením základného profilu zabezpečenia v službe Intune vytvoríte šablónu, ktorá sa skladá z viacerých profilov konfigurácie zariadenia.</span><span class="sxs-lookup"><span data-stu-id="488d9-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="488d9-106">Keď nasadíte základné údaje zabezpečenia do skupín používateľov alebo zariadení, nastavenia sa použijú na zariadenia spustené vo Windowse 10 alebo novších verziách.</span><span class="sxs-lookup"><span data-stu-id="488d9-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="488d9-107">Napríklad automatické vytvorenie pôvodného plánu Microsoft Mobile Device Management (MDM) (1) zapne funkciu BitLocker for vymeniteľných jednotiek, (2) vyžaduje heslo na odomknutie zariadenia a (3) zakáže základné overovanie.</span><span class="sxs-lookup"><span data-stu-id="488d9-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="488d9-108">Ak predvolená hodnota v prostredí nie je funkčná, môžete prispôsobiť základnú čiaru tak, aby používala požadované nastavenia.</span><span class="sxs-lookup"><span data-stu-id="488d9-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="488d9-109">Základné informácie o zabezpečení tiež pomáhajú pri vytváraní pracovného postupu koncového zabezpečenia v programe Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="488d9-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="488d9-110">Nižšie sú uvedené niektoré výhody tejto funkcie:</span><span class="sxs-lookup"><span data-stu-id="488d9-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="488d9-111">Základná hodnota zabezpečenia obsahuje najvhodnejšie postupy a odporúčania pre nastavenia, ktoré majú vplyv na zabezpečenie.</span><span class="sxs-lookup"><span data-stu-id="488d9-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="488d9-112">Keďže partneri služby Intune s tímom zabezpečenia systému Windows, ktorý vytvára základné hodnoty pre politiky skupiny, sú tieto odporúčania založené na solídnom poradenstve a rozsiahlych skúsenostiach.</span><span class="sxs-lookup"><span data-stu-id="488d9-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="488d9-113">Ak sa v službe Intune nachádzate a neviete, kde začať, základné informácie o zabezpečení vám pomôžu rýchlo vytvoriť a nasadiť zabezpečený profil.</span><span class="sxs-lookup"><span data-stu-id="488d9-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="488d9-114">Ak v súčasnosti používate skupinovú politiku, migrácia do služby Intune na účely správy je oveľa jednoduchšia s pôvodnými bezpečnostnými hodnotami, pretože tieto základné prvky zabezpečenia sú vstavané do služby Intune a obsahujú najmodernejšie možnosti spravovania.</span><span class="sxs-lookup"><span data-stu-id="488d9-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="488d9-115">Ďalšie informácie nájdete v téme [základné informácie o zabezpečení systému Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) a [Správa mobilných zariadení](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="488d9-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>