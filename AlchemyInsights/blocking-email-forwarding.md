---
title: Blokovanie alebo odblokovanie externého automatického preposielania e-mailov
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315889"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blokovanie alebo odblokovanie automatického preposielania e-mailov

Ak chcete zapnúť alebo vypnúť preposielanie e-mailov pre konkrétnu poštovú schránku, pozrite si časť [Konfigurácia preposielania e-mailov.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Správcovia môžu riadiť externé preposielanie pre organizáciu pomocou [politík odchádzajúcej nevyžiadanej pošty.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Politiky odchádzajúcej nevyžiadanej pošty môžete spravovať na portáli Microsoft 365 Defender na lokalite alebo pomocou rutiny <https://security.microsoft.com/antispam> typu cmdlet [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) v prostredí Exchange Online PowerShell.

Ak sa zobrazí nasledujúca chyba: **"550 5.7.520 Prístup odmietnutý,** Vaša organizácia nepovoľuje externé preposielanie", uistite sa, že politika je nakonfigurovaná tak, aby umožňovala externé automaticky preposielané správy.

**Poznámka:** Odporúčame predvolenú hodnotu Automaticky **–**  systém ovládaný nastavením pravidiel automatického presmerovania v predvolenej politike filtrovania odchádzajúcej nevyžiadanej pošty (automatické externé preposielanie je blokované, interné automatické preposielanie stále funguje). Mali by ste vytvoriť vlastné politiky filtrovania odchádzajúcej nevyžiadanej pošty a použiť hodnotu Zapnuté **–** preposielanie je povolené iba pre používateľov, ktorí potrebujú externé automatické preposielanie e-mailov. Ďalšie informácie nájdete v téme Konfigurácia [preposielania externých e-mailov Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
