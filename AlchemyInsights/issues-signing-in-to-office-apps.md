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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579952"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="eb0f0-102">Správa O nastavení aplikácie Microsoft 365 Ľutujeme, ďalšie konto z vašej organizácie je už prihlásený</span><span class="sxs-lookup"><span data-stu-id="eb0f0-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="eb0f0-103">Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:</span><span class="sxs-lookup"><span data-stu-id="eb0f0-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="eb0f0-104">Odstráňte všetky pracovné kontá okrem príslušného konta pomocou nastavení systému Windows > **accessovej práce alebo školy**.</span><span class="sxs-lookup"><span data-stu-id="eb0f0-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="eb0f0-105">[Vymažte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="eb0f0-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="eb0f0-106">**Upozornenie:** Cesty databázy registry pre Office 2016 sa zmenili na 16.0.</span><span class="sxs-lookup"><span data-stu-id="eb0f0-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="eb0f0-107">(Napr.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="eb0f0-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="eb0f0-108">Otvorte aplikáciu balíka Office a vyberte položku **File**  >  **Account**  >  **Odhláste sa**v konte súboru . Potom sa prihláste pomocou používateľského konta s platnou licenciou.</span><span class="sxs-lookup"><span data-stu-id="eb0f0-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="eb0f0-109">Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="eb0f0-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="eb0f0-110">V prípade Macu si pozrite tému [Nemôžem sa prihlásiť do aplikácie balíka Office 2016 pre Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="eb0f0-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="eb0f0-111">Ďalšie informácie nájdete v časti ["Ľutujeme, v tomto počítači je už prihlásenie iného konta z vašej organizácie" v balíku Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="eb0f0-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>