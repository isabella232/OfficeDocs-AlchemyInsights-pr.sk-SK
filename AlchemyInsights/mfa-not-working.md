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
# <a name="issues-with-mfa"></a>Problémy s makrofinančnej pomoci
Existuje niekoľko vecí na kontrolu, či používatelia nemôžu prihlásiť pomocou viacnásobné overovanie (MFA)

1. Postihnutého používateľa môže byť blokovaný v Azure Active Directory Portal. V takom prípade sa pokusy o overenie pre konkrétneho používateľa automaticky zamietnu. [Ak ich chcete odblokovať, postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ak odblokovanie používateľ nepomohlo, alebo používateľ nie je blokovaný, môžete skúsiť obnoviť MFA pre používateľa a budú prechádzať proces zapísať znova. [Prosím, postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ak je to prvýkrát, čo ste povolili MFA a vaši používatelia sa nemôžu prihlásiť na non-prehliadače klientov, ako je Outlook, Skype, atď, snáď ADAL (Active Directory Authentication Library) nie je povolená na vaše predplatné služby O365. V tomto prípade budete musieť pripojiť k službe Exchange Online PowerShell a spustiť túto rutinu cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*