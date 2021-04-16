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
# <a name="issues-with-azure-mfa"></a>Problémy so službou Azure MFA
Ak sa používatelia nemôžu prihlásiť pomocou viacfaktorového overovania (MFA), je potrebné skontrolovať niekoľko vecí.

1. Ovplyvnený používateľ môže byť zablokovaný na portáli Azure Active Directory. V takom prípade sa automaticky zamietli pokusy o overenie konkrétneho používateľa. [Ak ich chcete odblokovať, postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ak odblokovanie používateľa nepomálo alebo používateľ nie je zablokovaný, môžete sa pokúsiť obnoviť viac mfA používateľa a používateľ prejde procesom registrácie znova. [Postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ak mfA zapnete prvýkrát a vaši používatelia sa nedokážu prihlásiť do klientov mimo prehliadačov, ako je napríklad Outlook, Skype atď., v predplatnom služieb O365 pravdepodobne nie je povolená knižnica ADAL (Active Directory Authentication Library). V tomto prípade sa budete musieť pripojiť k službe Exchange Online v prostredí PowerShell a spustiť túto rutinu typu cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*