---
title: Problémy s prihlásením do aplikácií balíka Office
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763016"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="bffa0-102">Problémy s prihlásením do aplikácií balíka Office</span><span class="sxs-lookup"><span data-stu-id="bffa0-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="bffa0-103">Ak chcete opraviť problémy s prihlásením v aplikáciách balíka Office, vyskúšajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="bffa0-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="bffa0-104">Odstráňte všetky pracovné kontá okrem príslušného konta pomocou nastavenia systému Windows > **prístup k práci alebo škole**.</span><span class="sxs-lookup"><span data-stu-id="bffa0-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="bffa0-105">[Vymažte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="bffa0-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="bffa0-106">**Poznámka:** Cesty databázy Registry pre balík Office 2016 sa zmenili na 16,0.</span><span class="sxs-lookup"><span data-stu-id="bffa0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="bffa0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="bffa0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="bffa0-108">Otvorte aplikáciu balíka Office, vyberte položku**konto** >  **súboru** > **odhlásiť**. Potom sa prihláste pomocou používateľského konta s platnou licenciou.</span><span class="sxs-lookup"><span data-stu-id="bffa0-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="bffa0-109">Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="bffa0-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="bffa0-110">V prípade Macu si pozrite tému [Nemôžem sa prihlásiť do aplikácie balíka Office 2016 pre Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="bffa0-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="bffa0-111">Ak sa chyby pri pripájaní k Microsoft 365 pomocou Office 2013, povoliť moderné overovanie pre klienta Office.</span><span class="sxs-lookup"><span data-stu-id="bffa0-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="bffa0-112">Ďalšie informácie nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="bffa0-112">For more information, see:</span></span>
- [<span data-ttu-id="bffa0-113">Nemôžete sa prihlásiť do Microsoft 365, Azure alebo Intune</span><span class="sxs-lookup"><span data-stu-id="bffa0-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="bffa0-114">Problémy s pripojením v prihlásenie po aktualizácii na balík Office 2016 build 16.0.7967 v systéme Windows 10</span><span class="sxs-lookup"><span data-stu-id="bffa0-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="bffa0-115">"Ľutujeme, iný účet z vašej organizácie je už prihlásený na tomto počítači" v balíku Office</span><span class="sxs-lookup"><span data-stu-id="bffa0-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="bffa0-116">Riešenie problémov s prihlásením s Office moderné overovanie pri použití ADFS</span><span class="sxs-lookup"><span data-stu-id="bffa0-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)