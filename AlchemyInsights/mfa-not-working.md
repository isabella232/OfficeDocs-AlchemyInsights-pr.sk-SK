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
# <a name="issues-with-azure-mfa"></a>Problémy so službou Azure MFA
Existuje niekoľko vecí, ktoré môžete skontrolovať, či sa používatelia nemôžu prihlásiť pomocou viacnásobného overovania (MFA)

1. Ovplyvnený používateľ môže byť blokovaný v portáli Azure Active Directory Portal. Ak ide o tento prípad, pokusy o overenie pre konkrétneho používateľa sa automaticky odmietnu. [Ak ich chcete odblokovať, postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ak odblokovanie používateľa nepomohlo alebo používateľ nie je blokovaný, môžete sa pokúsiť o vytvorenie nového MFA pre používateľa a opätovne prejsť procesom registrácie. [Postupujte podľa krokov v tomto článku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ak sa vám po prvýkrát povolila MFA a používatelia sa nemôžu prihlásiť do neprehliadačov, akými sú napríklad Outlook, Skype atď., snad ADAL (Active Directory Authentication Library) nie je vo vašom predplatnom služieb O365 povolená. V tomto prípade sa budete musieť pripojiť k službe Exchange Online PowerShell a spustiť túto rutinu typu cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*