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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768852"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="7908e-102">Problémy s Azure MFA</span><span class="sxs-lookup"><span data-stu-id="7908e-102">Issues with Azure MFA</span></span>
<span data-ttu-id="7908e-103">Existuje niekoľko vecí skontrolovať, ak používatelia nemôžu prihlásiť pomocou viacnásobné overovanie (MFA)</span><span class="sxs-lookup"><span data-stu-id="7908e-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="7908e-104">Postihnutého používateľa môže byť blokovaný v Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="7908e-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="7908e-105">V takom prípade sa pokusy o overenie pre konkrétneho používateľa automaticky zamietnu.</span><span class="sxs-lookup"><span data-stu-id="7908e-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="7908e-106">Ak ich chcete odblokovať, postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="7908e-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="7908e-107">Ak odblokovanie používateľ nepomohlo, alebo používateľ nie je blokovaný, môžete skúsiť obnoviť MFA pre používateľa a budú prechádzať proces zapísať znova.</span><span class="sxs-lookup"><span data-stu-id="7908e-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="7908e-108">Prosím, postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="7908e-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="7908e-109">Ak je to prvýkrát, čo ste povolili MFA a vaši používatelia sa nemôžu prihlásiť na non-prehliadače klientov, ako je Outlook, Skype, atď, snáď ADAL (Active Directory Authentication Library) nie je povolená na vaše predplatné služby O365.</span><span class="sxs-lookup"><span data-stu-id="7908e-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="7908e-110">V tomto prípade budete musieť pripojiť k službe Exchange Online PowerShell a spustiť túto rutinu cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="7908e-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>