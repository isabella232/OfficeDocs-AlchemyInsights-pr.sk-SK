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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938334"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="9acb5-102">Problémy s prihlásením do aplikácie balíka Office</span><span class="sxs-lookup"><span data-stu-id="9acb5-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="9acb5-103">Vyriešiť prihlasovaním s kancelárskymi aplikáciami, vyskúšajte nasledujúci postup:</span><span class="sxs-lookup"><span data-stu-id="9acb5-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="9acb5-104">Odstráňte všetky pracovné účty, okrem postihnutých konta pomocou nastavenia systému Windows > **prístup k práci alebo v škole**.</span><span class="sxs-lookup"><span data-stu-id="9acb5-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="9acb5-105">[Jasné úradu poverení](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou poverení správcu systému Windows.</span><span class="sxs-lookup"><span data-stu-id="9acb5-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9acb5-106">**Poznámka:** Cesty databázy registry Office 2016 zmenili 16,0.</span><span class="sxs-lookup"><span data-stu-id="9acb5-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9acb5-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9acb5-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="9acb5-108">Otvorte aplikáciu balíka Office, vyberte **súbor** > **účet** > **Odhlásiť**. Potom sa prihláste pomocou používateľského konta s platnou licenciou.</span><span class="sxs-lookup"><span data-stu-id="9acb5-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="9acb5-109">Podrobné informácie nájdete v téme [kontá v kancelárii](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="9acb5-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="9acb5-110">Pre Mac, pozri [nemôžete prihlásiť do Office 2016 pre Mac aplikácie](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="9acb5-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="9acb5-111">Ak chyby sa vyskytuje pri pripájaní k Office 365 pomocou Office 2013, umožňujú moderné overenie Office klienta.</span><span class="sxs-lookup"><span data-stu-id="9acb5-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="9acb5-112">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="9acb5-112">For more information, see:</span></span>
- [<span data-ttu-id="9acb5-113">Nemôžete prihlásiť k Office 365, Azure alebo Intune</span><span class="sxs-lookup"><span data-stu-id="9acb5-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="9acb5-114">Problémy s pripojením v sign-in po aktualizácii Office 2016 build 16.0.7967 v systéme Windows 10</span><span class="sxs-lookup"><span data-stu-id="9acb5-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="9acb5-115">"Prepáč, iný účet z vašej organizácie je už prihlásený na tomto počítači" v kancelárii</span><span class="sxs-lookup"><span data-stu-id="9acb5-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="9acb5-116">Riešenie problémov prihlasovacích Office moderných overovanie pri používaní ADFS</span><span class="sxs-lookup"><span data-stu-id="9acb5-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)