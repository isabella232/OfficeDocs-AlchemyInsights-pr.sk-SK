---
title: 726 Blokovanie preposielanie e-mailov
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059647"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokovanie alebo odblokovanie preposielania e-mailov

Ak chcete zapnúť alebo vypnúť preposielanie e-mailov pre konkrétnu poštovú schránku, pozrite si časť [Konfigurácia preposielania e-mailov.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Na úrovni nájomníka sa kontrola externého preposielania vykonáva pomocou politiky odchádzajúcej nevyžiadanej pošty. Politiku filtrovania odchádzajúcej nevyžiadanej pošty si [](https://protection.office.com/antispam) môžete pozrieť z Centra zabezpečenia a dodržiavania súladu tu alebo pomocou príkazu [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Ak sa zobrazí nasledujúca chyba: **"550 5.7.520 Prístup odmietnutý,** Vaša organizácia neumožňuje externé preposielanie", uistite sa, že politika je nakonfigurovaná tak, aby umožňovala externé automatické preposielanie.

**Poznámka:** V predvolenej politike filtrovania odchádzajúcej nevyžiadanej pošty sa odporúča ponechať vypnutú externú funkciu automatického dokončovania a povoliť ju len používateľom, ktorí potrebujú externé preposielanie, a to vytvorením vlastnej politiky pre týchto používateľov. Ďalšie informácie nájdete v článku Konfigurácia [preposielanie externých e-mailov v Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)