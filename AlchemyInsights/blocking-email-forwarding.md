---
title: 726 blokovanie preposielania e-mailov
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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219870"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokovanie alebo odblokovanie preposielania e-mailov

Ak chcete zapnúť alebo vypnúť presmerovanie e-mailov pre konkrétnu poštovú schránku, prečítajte si tému [Konfigurácia preposielania](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Na úrovni nájomníka sa kontrola externého preposielania uskutočňuje pomocou odchádzajúcej politiky ochrany pred nevyžiadanou poštou. Ak je nastavená na možnosť vypnutá alebo automatická, môže blokovať preposielanie e-mailov s odmietnutým prístupom "550 5.7.520, vaša organizácia nepovoľuje externé preposielanie". Následne, ak bolo preposielanie nastavené na možnosť blokované, znamená to chybu, ktorú budú používatelia zobrazovať.

Ak je presmerovanie zablokované, skontrolujte, či je politika nakonfigurovaná na povolenie externého preposielania. Odchádzajúca politika filtrovania nevyžiadanej pošty môžete skontrolovať v centre zabezpečenia a dodržiavania súladu alebo spustením príkazu Get-HostedOutboundSpamFilterPolicy | FL Name, AutoForwardingMode. Ak chcete nastaviť blokovanie automaticky preposielaných údajov, rovnaký príkaz vám oznámi stav politiky.

Poznámka: odporúča sa ponechať externé automatické preposielanie vypnuté v predvolenej politike filtra odchádzajúcich nevyžiadanej pošty a povoliť ho len používateľom, ktorí potrebujú externé preposielanie, a to vytvorením vlastnej politiky pre týchto používateľov. Ďalšie informácie nájdete v téme [Konfigurácia externého preposielania e-mailov v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).