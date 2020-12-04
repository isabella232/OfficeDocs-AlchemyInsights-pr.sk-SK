---
title: Použitie pôvodných plánov zabezpečenia služby Microsoft Intune na konfiguráciu zariadení s Windowsom 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573531"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="1c0ee-102">Použitie pôvodných plánov zabezpečenia služby Microsoft Intune na konfiguráciu zariadení s Windowsom 10</span><span class="sxs-lookup"><span data-stu-id="1c0ee-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="1c0ee-103">Základné údaje zabezpečenia služby Intune pomáhajú chrániť používateľov a zariadenia.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="1c0ee-104">Základné údaje zabezpečenia sú predkonfigurované skupiny nastavení Windowsu, ktoré sa používajú na použitie známej skupiny nastavení a predvolených hodnôt odporúčaných príslušnými tímami zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="1c0ee-105">Vytvorením základného profilu zabezpečenia v službe Intune vytvoríte šablónu, ktorá sa skladá z viacerých profilov konfigurácie zariadenia.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="1c0ee-106">Keď nasadíte základné hodnoty zabezpečenia do skupín používateľov alebo zariadení, nastavenia sa použijú na zariadenia spustené vo Windowse 10 alebo novšom.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="1c0ee-107">Napríklad funkcia MDM Security Baseline automaticky (1) zapne funkciu BitLocker for vymeniteľných jednotiek, (2) vyžaduje heslo na odomknutie zariadenia a (3) zakáže základné overovanie.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="1c0ee-108">Ak predvolená hodnota v prostredí nie je funkčná, prispôsobte základnú čiaru tak, aby sa aplikovali potrebné nastavenia.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="1c0ee-109">Základné informácie o zabezpečení tiež pomáhajú pri vytváraní pracovného postupu koncového zabezpečenia v programe Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="1c0ee-110">Nižšie sú uvedené niektoré výhody tohto:</span><span class="sxs-lookup"><span data-stu-id="1c0ee-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="1c0ee-111">Základná hodnota zabezpečenia obsahuje najvhodnejšie postupy a odporúčania pre nastavenia, ktoré majú vplyv na zabezpečenie.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="1c0ee-112">Keďže partneri služby Intune s tímom zabezpečenia systému Windows, ktorý vytvára základné hodnoty pre politiky skupiny, sú tieto odporúčania založené na solídnom poradenstve a rozsiahlych skúsenostiach.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="1c0ee-113">Ak sa v službe Intune nachádzate a neviete, kde začať, základné informácie o zabezpečení vám pomôžu rýchlo vytvoriť a nasadiť zabezpečený profil.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="1c0ee-114">Ak v súčasnosti používate skupinovú politiku, migrácia do služby Intune na účely správy je oveľa jednoduchšia so základmi zabezpečenia, pretože sú zabudované do služby Intune a obsahujú najmodernejšie možnosti spravovania.</span><span class="sxs-lookup"><span data-stu-id="1c0ee-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="1c0ee-115">Ďalšie informácie nájdete v téme [základné informácie o zabezpečení systému Windows](https://go.microsoft.com/fwlink/?linkid=2141503) a [Správa mobilných zariadení](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="1c0ee-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>