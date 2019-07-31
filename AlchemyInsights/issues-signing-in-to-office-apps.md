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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938333"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="263f5-102">Stanovenie Office apps "Prepáč, iný účet z vašej organizácie je už prihlásený" hlásenie</span><span class="sxs-lookup"><span data-stu-id="263f5-102">Fixing the Office apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="263f5-103">Opraviť túto chybu, skúste nasledujúce:</span><span class="sxs-lookup"><span data-stu-id="263f5-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="263f5-104">Odstráňte všetky pracovné účty, okrem postihnutých konta pomocou nastavenia systému Windows > **prístup k práci alebo v škole**.</span><span class="sxs-lookup"><span data-stu-id="263f5-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="263f5-105">[Jasné úradu poverení](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou poverení správcu systému Windows.</span><span class="sxs-lookup"><span data-stu-id="263f5-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="263f5-106">**Poznámka:** Cesty databázy registry Office 2016 zmenili 16,0.</span><span class="sxs-lookup"><span data-stu-id="263f5-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="263f5-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="263f5-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="263f5-108">Otvorte aplikáciu balíka Office, vyberte **súbor** > **účet** > **Odhlásiť**. Potom sa prihláste pomocou používateľského konta s platnou licenciou.</span><span class="sxs-lookup"><span data-stu-id="263f5-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="263f5-109">Podrobné informácie nájdete v téme [kontá v kancelárii](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="263f5-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="263f5-110">Pre Mac, pozri [nemôžete prihlásiť do Office 2016 pre Mac aplikácie](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="263f5-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="263f5-111">Ďalšie informácie nájdete v téme ["Ospravedlňujeme sa, iný účet z vašej organizácie je už prihlásený na tomto počítači" vo funkcii](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="263f5-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>