---
title: Problémy s prihlásením do aplikácie balíka Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938336"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="43e10-102">Stanovenie Office apps "Trusted Platform module počítača nepracuje správne" správy</span><span class="sxs-lookup"><span data-stu-id="43e10-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="43e10-103">Opraviť túto chybu, skúste nasledujúce:</span><span class="sxs-lookup"><span data-stu-id="43e10-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="43e10-104">Nainštalujte najnovšie aktualizácie pre [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="43e10-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="43e10-105">[Jasné úradu poverení](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou poverení správcu systému Windows.</span><span class="sxs-lookup"><span data-stu-id="43e10-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="43e10-106">**Poznámka:** Cesty databázy registry Office 2016 zmenili 16,0.</span><span class="sxs-lookup"><span data-stu-id="43e10-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="43e10-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="43e10-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="43e10-108">Skúste [používateľa ozdravný proces](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) opraviť zlyhania Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="43e10-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="43e10-109">Nastaviť EnableADAL = 0 pomocou nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="43e10-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="43e10-110">Kliknite pravým tlačidlom myši na tlačidlo Štart, vyberte **Spustiť**, zadajte **príkaz regedit**a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="43e10-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="43e10-111">Vyberte **Áno** povoliť Editor databázy Registry zmeny do vášho zariadenia.</span><span class="sxs-lookup"><span data-stu-id="43e10-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="43e10-112">V editore databázy Registry pridajte hodnotu DWORD **EnableADAL** s nastavením **0** pod HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="43e10-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="43e10-113">Ďalšie informácie nájdete v téme [pripojenie problémy v sign-in po aktualizácii Office 2016 build 16.0.7967 v systéme Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="43e10-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>