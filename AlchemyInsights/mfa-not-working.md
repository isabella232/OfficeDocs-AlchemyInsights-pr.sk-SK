---
title: Problémy s MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755146"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="52bde-102">Problémy so službou Azure MFA</span><span class="sxs-lookup"><span data-stu-id="52bde-102">Issues with Azure MFA</span></span>
<span data-ttu-id="52bde-103">Existuje niekoľko vecí, ktoré môžete skontrolovať, či sa používatelia nemôžu prihlásiť pomocou viacnásobného overovania (MFA)</span><span class="sxs-lookup"><span data-stu-id="52bde-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="52bde-104">Ovplyvnený používateľ môže byť blokovaný v portáli Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="52bde-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="52bde-105">Ak ide o tento prípad, pokusy o overenie pre konkrétneho používateľa sa automaticky odmietnu.</span><span class="sxs-lookup"><span data-stu-id="52bde-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="52bde-106">Ak ich chcete odblokovať, postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="52bde-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="52bde-107">Ak odblokovanie používateľa nepomohlo alebo používateľ nie je blokovaný, môžete sa pokúsiť o vytvorenie nového MFA pre používateľa a opätovne prejsť procesom registrácie.</span><span class="sxs-lookup"><span data-stu-id="52bde-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="52bde-108">Postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="52bde-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="52bde-109">Ak sa vám po prvýkrát povolila MFA a používatelia sa nemôžu prihlásiť do neprehliadačov, akými sú napríklad Outlook, Skype atď., snad ADAL (Active Directory Authentication Library) nie je vo vašom predplatnom služieb O365 povolená.</span><span class="sxs-lookup"><span data-stu-id="52bde-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="52bde-110">V tomto prípade sa budete musieť pripojiť k službe Exchange Online PowerShell a spustiť túto rutinu typu cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="52bde-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>