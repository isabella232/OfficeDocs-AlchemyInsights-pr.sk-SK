---
title: Problémy s MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810499"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="3e597-102">Problémy so službou Azure MFA</span><span class="sxs-lookup"><span data-stu-id="3e597-102">Issues with Azure MFA</span></span>
<span data-ttu-id="3e597-103">Ak sa používatelia nemôžu prihlásiť pomocou viacfaktorového overovania (MFA), je potrebné skontrolovať niekoľko vecí.</span><span class="sxs-lookup"><span data-stu-id="3e597-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="3e597-104">Ovplyvnený používateľ môže byť zablokovaný na portáli Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3e597-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="3e597-105">V takom prípade sa automaticky zamietli pokusy o overenie konkrétneho používateľa.</span><span class="sxs-lookup"><span data-stu-id="3e597-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="3e597-106">Ak ich chcete odblokovať, postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="3e597-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="3e597-107">Ak odblokovanie používateľa nepomálo alebo používateľ nie je zablokovaný, môžete sa pokúsiť obnoviť viac mfA používateľa a používateľ prejde procesom registrácie znova.</span><span class="sxs-lookup"><span data-stu-id="3e597-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="3e597-108">Postupujte podľa krokov v tomto článku.</span><span class="sxs-lookup"><span data-stu-id="3e597-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="3e597-109">Ak mfA zapnete prvýkrát a vaši používatelia sa nedokážu prihlásiť do klientov mimo prehliadačov, ako je napríklad Outlook, Skype atď., v predplatnom služieb O365 pravdepodobne nie je povolená knižnica ADAL (Active Directory Authentication Library).</span><span class="sxs-lookup"><span data-stu-id="3e597-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="3e597-110">V tomto prípade sa budete musieť pripojiť k službe Exchange Online v prostredí PowerShell a spustiť túto rutinu typu cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="3e597-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>