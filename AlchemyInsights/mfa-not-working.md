---
title: Problémy s MZV
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545195"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="e7760-102">Problémy s MZV</span><span class="sxs-lookup"><span data-stu-id="e7760-102">Issues with MFA</span></span>
<span data-ttu-id="e7760-103">Existuje pár vecí na kontrolu, ak užívatelia nemôžu prihlásiť pomocou viacnásobné overovanie (MFA)</span><span class="sxs-lookup"><span data-stu-id="e7760-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="e7760-104">Príslušného používateľa môže byť zablokovaný v portáli Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e7760-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="e7760-105">Ak je tomu tak, overovacie pokusy, že konkrétny používateľ bude automaticky zamietnutý.</span><span class="sxs-lookup"><span data-stu-id="e7760-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="e7760-106">Postupujte podľa krokov v tomto článku a ich odblokovanie.</span><span class="sxs-lookup"><span data-stu-id="e7760-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="e7760-107">Ak nepomohlo, odblokovanie používateľa alebo používateľ nie je blokovaný môžete skúsiť obnoviť MFA pre používateľa a pôjdu cez proces registrovať znova.</span><span class="sxs-lookup"><span data-stu-id="e7760-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="e7760-108">Postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="e7760-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="e7760-109">Ak je to prvýkrát, čo ste MZV zapnuté a používatelia schopní prihlásiť-prehliadače klientov ako je Outlook, Skype, atď, možno ADAL (Active Directory overenie knižnica) nie je povolená na odber služby O365.</span><span class="sxs-lookup"><span data-stu-id="e7760-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="e7760-110">V tomto prípade budete musieť pripojiť k Exchange Online Powershell a spustite tento cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="e7760-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>