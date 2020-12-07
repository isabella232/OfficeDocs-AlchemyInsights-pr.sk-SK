---
title: Microsoft Edge Support pre aplikáciu Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584011"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="7c9d2-102">Microsoft Edge Support pre aplikáciu Microsoft Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="7c9d2-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="7c9d2-103">Aplikácia Guard je navrhnutá pre Windows 10 a Microsoft Edge, ktorá používa hardvérový izolačný prístup, ktorý umožňuje používateľovi prejsť na nedôveryhodnú lokalitu zvnútra izolovaného, Hyper-V-povoleného kontajnera oddeleného od hostiteľského operačného systému.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="7c9d2-104">Podnikový správca definuje zoznam dôveryhodných webových lokalít, cloudových zdrojov a interných sietí.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="7c9d2-105">Keď používateľ navštívi lokalitu, ktorá sa nenachádza v zozname, Microsoft Edge otvorí lokalitu v kontajneri.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="7c9d2-106">To znamená, že ak sa lokalita ukáže ako škodlivá, hostiteľský počítač zostane zabezpečený a útočník sa nedostane do podnikových údajov.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="7c9d2-107">Inštalácia rozšírení v kontajneri je podporovaná v prehliadači Microsoft Edge verzie 81 a môže byť riadená prostredníctvom politiky.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="7c9d2-108">Adresa updateURL, ktorá sa použije v politike ExtensionInstallForcelist, by sa mala pridať ako neutrálny zdroj v politike izolácie siete, ktorú používa strážca aplikácie.</span><span class="sxs-lookup"><span data-stu-id="7c9d2-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="7c9d2-109">Ďalšie informácie nájdete v téme [podpora aplikácie Microsoft Edge pre aplikáciu Microsoft Defender Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="7c9d2-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
