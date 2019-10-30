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
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768852"
---
# <a name="issues-with-azure-mfa"></a>Problémy s Azure MFA
Existuje niekoľko vecí skontrolovať, ak používatelia nemôžu prihlásiť pomocou viacnásobné overovanie (MFA)

1. Postihnutého používateľa môže byť blokovaný v Azure Active Directory Portal. V takom prípade sa pokusy o overenie pre konkrétneho používateľa automaticky zamietnu. [Ak ich chcete odblokovať, postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ak odblokovanie používateľ nepomohlo, alebo používateľ nie je blokovaný, môžete skúsiť obnoviť MFA pre používateľa a budú prechádzať proces zapísať znova. [Prosím, postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ak je to prvýkrát, čo ste povolili MFA a vaši používatelia sa nemôžu prihlásiť na non-prehliadače klientov, ako je Outlook, Skype, atď, snáď ADAL (Active Directory Authentication Library) nie je povolená na vaše predplatné služby O365. V tomto prípade budete musieť pripojiť k službe Exchange Online PowerShell a spustiť túto rutinu cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*