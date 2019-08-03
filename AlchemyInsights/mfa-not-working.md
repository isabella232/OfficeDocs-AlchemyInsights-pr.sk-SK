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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250180"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="ef1a9-102">Problémy s MZV</span><span class="sxs-lookup"><span data-stu-id="ef1a9-102">Issues with MFA</span></span>
<span data-ttu-id="ef1a9-103">Existuje pár vecí na kontrolu, ak užívatelia nemôžu prihlásiť pomocou viacnásobné overovanie (MFA)</span><span class="sxs-lookup"><span data-stu-id="ef1a9-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="ef1a9-104">Príslušného používateľa môže byť zablokovaný v portáli Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ef1a9-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="ef1a9-105">Ak je tomu tak, overovacie pokusy, že konkrétny používateľ bude automaticky zamietnutý.</span><span class="sxs-lookup"><span data-stu-id="ef1a9-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="ef1a9-106">Postupujte podľa krokov v tomto článku a ich odblokovanie.</span><span class="sxs-lookup"><span data-stu-id="ef1a9-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="ef1a9-107">Ak nepomohlo, odblokovanie používateľa alebo používateľ nie je blokovaný môžete skúsiť obnoviť MFA pre používateľa a pôjdu cez proces registrovať znova.</span><span class="sxs-lookup"><span data-stu-id="ef1a9-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="ef1a9-108">Postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="ef1a9-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="ef1a9-109">Ak je to prvýkrát, čo ste MZV zapnuté a používatelia schopní prihlásiť-prehliadače klientov ako je Outlook, Skype, atď, možno ADAL (Active Directory overenie knižnica) nie je povolená na odber služby O365.</span><span class="sxs-lookup"><span data-stu-id="ef1a9-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="ef1a9-110">V tomto prípade budete musieť pripojiť k Exchange Online Powershell a spustite tento cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="ef1a9-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>