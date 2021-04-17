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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833090"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="c7944-102">Oprava správy o aplikáciách služby Microsoft 365 "Ľutujeme, iné konto z vašej organizácie je už prihlásené"</span><span class="sxs-lookup"><span data-stu-id="c7944-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="c7944-103">Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:</span><span class="sxs-lookup"><span data-stu-id="c7944-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="c7944-104">Odstráňte všetky pracovné kontá s výnimkou príslušného konta pomocou nastavení Windowsu > **prístup k pracovnom alebo školskému kontu.**</span><span class="sxs-lookup"><span data-stu-id="c7944-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="c7944-105">[Odstráňte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.</span><span class="sxs-lookup"><span data-stu-id="c7944-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c7944-106">**Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na hodnotu 16.0.</span><span class="sxs-lookup"><span data-stu-id="c7944-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c7944-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c7944-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c7944-108">Otvorte aplikáciu balíka Office a vyberte položku  >  **Odhlásiť**  >  **sa konto súboru**. Potom sa prihláste pomocou používateľského konta s platnou licenciou.</span><span class="sxs-lookup"><span data-stu-id="c7944-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="c7944-109">Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="c7944-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="c7944-110">V prípade Macu si pozrite tému [Nemôžem sa prihlásiť do aplikácie balíka Office 2016 pre Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="c7944-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="c7944-111">Ďalšie informácie nájdete v téme [Ľutujeme, iné konto z vašej organizácie je už v tomto počítači prihlásené v Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="c7944-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>