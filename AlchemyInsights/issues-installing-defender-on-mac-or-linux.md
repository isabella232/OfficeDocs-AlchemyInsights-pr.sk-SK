---
title: Problémy s inštaláciou aplikácie Microsoft Defender v Macu alebo Linuxe
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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539695"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="f0bab-102">Problémy s inštaláciou aplikácie Microsoft Defender v Macu alebo Linuxe</span><span class="sxs-lookup"><span data-stu-id="f0bab-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="f0bab-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="f0bab-103">**Mac**</span></span>

- <span data-ttu-id="f0bab-104">Pred inštaláciou balíka Microsoft Defender ATP Mac skontrolujte, či sú splnené systémové požiadavky.</span><span class="sxs-lookup"><span data-stu-id="f0bab-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="f0bab-105">Ďalšie informácie nájdete v téme [Inštalácia balíka Microsoft Defender ATP pre Mac.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="f0bab-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="f0bab-106">Skontrolujte informácie v súbore: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="f0bab-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="f0bab-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="f0bab-107">**Linux**</span></span>

- <span data-ttu-id="f0bab-108">Pred inštaláciou Linuxu skontrolujte, či sú Microsoft Defender ATP splnené systémové požiadavky.</span><span class="sxs-lookup"><span data-stu-id="f0bab-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="f0bab-109">Ďalšie informácie nájdete v téme [Ako nainštalovať MDATP pre Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="f0bab-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="f0bab-110">Ak chcete overiť, či je spustená služba MDATP, pozrite si časť [Inštalácia zlyhala.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="f0bab-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="f0bab-111">Ak chcete riešiť a riešiť problémy, ak služba nie je spustená, pozrite si tému Kroky na [riešenie problémov, ak služba MDATP nie je spustená.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="f0bab-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="f0bab-112">Kroky na kontrolu konfigurácie klienta, overenie stavu produktu a spustenie testu zisťovania v textovom súbore systému EICAR nájdete v téme [Konfigurácia klienta.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="f0bab-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="f0bab-113">**Poznámka** Zoznam podporovaných systémov súborov pre aktivitu pri prístupe nájdete v téme [Microsoft Defender ATP pre Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="f0bab-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>