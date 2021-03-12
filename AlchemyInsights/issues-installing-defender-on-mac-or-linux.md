---
title: Problémy s inštaláciou programu Microsoft Defender v Macu alebo Linuxe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713845"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="d8519-102">Problémy s inštaláciou programu Microsoft Defender v Macu alebo Linuxe</span><span class="sxs-lookup"><span data-stu-id="d8519-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="d8519-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="d8519-103">**Mac**</span></span>

- <span data-ttu-id="d8519-104">Pred nainštalovaním aplikácie Microsoft Defender ATP pre Mac Skontrolujte, či sú splnené systémové požiadavky.</span><span class="sxs-lookup"><span data-stu-id="d8519-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="d8519-105">Ďalšie informácie nájdete v téme [Inštalácia programu Microsoft Defender ATP pre Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="d8519-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="d8519-106">Skontrolujte informácie v súbore: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="d8519-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="d8519-107">**Linuxe**</span><span class="sxs-lookup"><span data-stu-id="d8519-107">**Linux**</span></span>

- <span data-ttu-id="d8519-108">Pred nainštalovaním aplikácie Microsoft Defender ATP pre Linux Skontrolujte, či sú splnené systémové požiadavky.</span><span class="sxs-lookup"><span data-stu-id="d8519-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="d8519-109">Ďalšie informácie nájdete v téme [Inštalácia programu Microsoft Defender ATP pre Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="d8519-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="d8519-110">Ak chcete overiť, či je spustená služba MDATP, pozrite si tému [Inštalácia zlyhala](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span><span class="sxs-lookup"><span data-stu-id="d8519-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="d8519-111">Ak chcete riešiť problémy a riešiť problémy, ak nie je spustená služba, pozrite si [postup pri riešení problémov, ak nie je spustená služba mdatp](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="d8519-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="d8519-112">Postup na kontrolu konfigurácie klienta, ktorý overí stav produktu, a spustite test zisťovania v textovom súbore EICAR, pozrite si tému [Konfigurácia klienta](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="d8519-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="d8519-113">**Poznámka:** Zoznam podporovaných súborových systémov pre aktivitu v Accesse nájdete v téme [Microsoft Defender ATP pre Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="d8519-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>