---
title: Problémy pri prihlasovaní do aplikácií Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833030"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="d2c7f-102">Hlásenie o oprave aplikácií služby Microsoft 365 "Modul dôveryhodnej platformy vášho počítača nefunkčný správne"</span><span class="sxs-lookup"><span data-stu-id="d2c7f-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="d2c7f-103">Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:</span><span class="sxs-lookup"><span data-stu-id="d2c7f-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d2c7f-104">Nainštalujte najnovšie aktualizácie pre [Windows a](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="d2c7f-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d2c7f-105">[Odstráňte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="d2c7f-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d2c7f-106">**Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na hodnotu 16.0.</span><span class="sxs-lookup"><span data-stu-id="d2c7f-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d2c7f-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d2c7f-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d2c7f-108">Skúste v [procese obnovenia používateľa](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) opraviť zlyhanie Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="d2c7f-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="d2c7f-109">Nastavte položku EnableADAL = 0 pomocou týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="d2c7f-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="d2c7f-110">Kliknite pravým tlačidlom myši na tlačidlo Štart vo Windowse, vyberte **položku Spustiť**, zadajte **príkaz regedit** a potom vyberte tlačidlo **OK.**</span><span class="sxs-lookup"><span data-stu-id="d2c7f-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="d2c7f-111">Ak **chcete editoru** databázy Registry povoliť vykonávať zmeny v zariadení, vyberte možnosť Áno.</span><span class="sxs-lookup"><span data-stu-id="d2c7f-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="d2c7f-112">V Editore databázy Registry pridajte hodnotu DWORD **položky EnableADAL** s nastavením **0 v** časti HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="d2c7f-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="d2c7f-113">Ďalšie informácie nájdete v téme Problémy s pripojením pri prihlasovaní po aktualizácii na [zostavu 16.0.7967 balíka Office 2016 vo Windowse 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="d2c7f-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>