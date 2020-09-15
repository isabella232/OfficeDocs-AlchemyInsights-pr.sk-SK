---
title: Problémy s prihlásením do aplikácií Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695194"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="e8480-102">Oprava aplikácií Microsoft 365 "Trusted Platform Module počítača nefunguje správne" správa</span><span class="sxs-lookup"><span data-stu-id="e8480-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="e8480-103">Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:</span><span class="sxs-lookup"><span data-stu-id="e8480-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="e8480-104">Nainštalujte si najnovšie aktualizácie pre [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="e8480-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="e8480-105">[Vymazanie poverení balíka Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="e8480-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e8480-106">**Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na 16,0.</span><span class="sxs-lookup"><span data-stu-id="e8480-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e8480-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e8480-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e8480-108">Vyskúšajte [proces obnovenia používateľa](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) na opravu zlyhaní modulu TPM (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="e8480-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="e8480-109">Nastavte Povoliťadal = 0 pomocou týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="e8480-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="e8480-110">Kliknite pravým tlačidlom myši na tlačidlo Štart systému Windows, vyberte položku **Spustiť**, zadajte **príkaz regedit**a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="e8480-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="e8480-111">Vyberte možnosť **Áno** , ak chcete povoliť Editor databázy Registry vykonávať zmeny v zariadení.</span><span class="sxs-lookup"><span data-stu-id="e8480-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="e8480-112">V editore databázy Registry pridajte hodnotu DWORD **povoliťadal** s nastavením **0** v časti HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="e8480-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="e8480-113">Ďalšie informácie nájdete v téme [problémy s pripojením pri prihlasovaní po aktualizácii na Office 2016 build 16.0.7967 vo Windowse 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="e8480-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>