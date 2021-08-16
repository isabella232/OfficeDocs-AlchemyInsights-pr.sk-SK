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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098617"
---
# <a name="issues-with-azure-mfa"></a>Problémy so službou Azure MFA
Ak sa používatelia nemôžu prihlásiť pomocou viacfaktorového overovania (MFA), je potrebné skontrolovať niekoľko vecí.

1. Ovplyvnený používateľ môže byť na portáli Azure Active Directory zablokovaný. V takom prípade sa automaticky zamietli pokusy o overenie konkrétneho používateľa. [Ak ich chcete odblokovať, postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ak odblokovanie používateľa nepomálo alebo používateľ nie je zablokovaný, môžete sa pokúsiť obnoviť viac mfA používateľa a používateľ prejde procesom registrácie znova. [Postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ak ste mfa po prvýkrát povolili a používatelia sa nedokážu prihlásiť do klientov mimo prehliadačov, ako sú napríklad Outlook, Skype atď. napríklad ADAL (Active Directory Authentication Library) nie je vo vašom predplatnom služieb O365 povolené. V tomto prípade sa budete musieť pripojiť k Exchange Online PowerShell a spustiť túto rutinu typu cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*