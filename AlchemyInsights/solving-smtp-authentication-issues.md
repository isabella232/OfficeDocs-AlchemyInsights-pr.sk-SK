---
title: Riešenie problémov s overním SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826430"
---
# <a name="solving-smtp-authentication-issues"></a>Riešenie problémov s overním SMTP

Ak sa pri pokuse o odoslanie e-mailu SMTP a overenie pomocou klienta alebo aplikácie zobrazí chyba 5.7.57 alebo 5.7.3, mali by ste skontrolovať niekoľko vecí:

- Overené odosielanie SMTP servera môže byť v nájomníkovi vypnuté alebo v poštovej schránke, ktorú sa pokúšate použiť (skontrolujte obe nastavenia). Ďalšie informácie nájdete v téme [Zapnutie alebo vypnutie odoslaného overeného klienta SMTP.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Skontrolujte, [či sú pre vášho nájomníka](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) povolené predvolené nastavenia zabezpečenia služby Azure. ak je povolené, overenie SMTP pomocou základného overovania (známe aj ako staršie verzie), ktoré použije meno používateľa a heslo, zlyhá.
