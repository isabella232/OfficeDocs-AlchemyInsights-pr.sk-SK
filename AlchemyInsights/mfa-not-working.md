---
title: Problémy s makrofinančnej pomoci
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545195"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="1b0d2-102">Problémy s makrofinančnej pomoci</span><span class="sxs-lookup"><span data-stu-id="1b0d2-102">Issues with MFA</span></span>
<span data-ttu-id="1b0d2-103">Existuje niekoľko vecí na kontrolu, či používatelia nemôžu prihlásiť pomocou viacnásobné overovanie (MFA)</span><span class="sxs-lookup"><span data-stu-id="1b0d2-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="1b0d2-104">Postihnutého používateľa môže byť blokovaný v Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="1b0d2-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="1b0d2-105">V takom prípade sa pokusy o overenie pre konkrétneho používateľa automaticky zamietnu.</span><span class="sxs-lookup"><span data-stu-id="1b0d2-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="1b0d2-106">Ak ich chcete odblokovať, postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="1b0d2-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="1b0d2-107">Ak odblokovanie používateľ nepomohlo, alebo používateľ nie je blokovaný, môžete skúsiť obnoviť MFA pre používateľa a budú prechádzať proces zapísať znova.</span><span class="sxs-lookup"><span data-stu-id="1b0d2-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="1b0d2-108">Prosím, postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="1b0d2-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="1b0d2-109">Ak je to prvýkrát, čo ste povolili MFA a vaši používatelia sa nemôžu prihlásiť na non-prehliadače klientov, ako je Outlook, Skype, atď, snáď ADAL (Active Directory Authentication Library) nie je povolená na vaše predplatné služby O365.</span><span class="sxs-lookup"><span data-stu-id="1b0d2-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="1b0d2-110">V tomto prípade budete musieť pripojiť k službe Exchange Online PowerShell a spustiť túto rutinu cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="1b0d2-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>