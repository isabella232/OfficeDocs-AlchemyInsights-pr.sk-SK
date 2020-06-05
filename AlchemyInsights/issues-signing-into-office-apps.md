---
title: Problémy s prihlásením do aplikácií Microsoft 365
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
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579880"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="abb2d-102">Oprava správy microsoft 365 aplikácie "Modul dôveryhodnej platformy počítača nefunguje správne"</span><span class="sxs-lookup"><span data-stu-id="abb2d-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="abb2d-103">Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:</span><span class="sxs-lookup"><span data-stu-id="abb2d-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="abb2d-104">Nainštalujte najnovšie aktualizácie pre [systém Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="abb2d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="abb2d-105">[Vymažte poverenia balíka Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="abb2d-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="abb2d-106">**Upozornenie:** Cesty databázy registry pre Office 2016 sa zmenili na 16.0.</span><span class="sxs-lookup"><span data-stu-id="abb2d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="abb2d-107">(Napr.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="abb2d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="abb2d-108">Skúste [proces obnovenia používateľa](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) opraviť zlyhania modulu TPM (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="abb2d-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="abb2d-109">Nastavte EnableADAL = 0 pomocou nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="abb2d-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="abb2d-110">Kliknite pravým tlačidlom myši na tlačidlo Štart systému Windows, vyberte položku **Spustiť**, zadajte **príkaz regedit**a potom vyberte tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="abb2d-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="abb2d-111">Ak chcete, aby Editor databázy Registry mohol vykonávať zmeny v zariadení, vyberte možnosť **Áno.**</span><span class="sxs-lookup"><span data-stu-id="abb2d-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="abb2d-112">V Editore databázy Registry pridajte hodnotu DWORD **EnableADAL** s nastavením **0** v HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="abb2d-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="abb2d-113">Ďalšie informácie nájdete v téme [Problémy s pripojením pri prihlasovaní po aktualizácii office 2016 stavať 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="abb2d-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>