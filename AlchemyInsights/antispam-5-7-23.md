---
title: Antispam – 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821426"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Odstránenie problémov s doručovaním e-mailov s kódom chyby 5.7.23

Overte SPF DNS záznam svojej domény na verejne dostupnej kontrole SPF alebo DNS záznamu na webe.

Overte, či spoločnosť Microsoft nei už odchádzajúca správa nebola identifikovaná ako nevyžiadaná pošta a smerovala cez Fond doručovania [s vysokým rizikom.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Správy z fondu doručovania s vysokým rizikom neprejdú kontrolami SPF, a preto ich cieľová e-mailová organizácia nebude prijímať.

Ak problém pretrváva, možno bude potrebné obrátiť sa na správcu poštového hostiteľa, ktorému sa pokúšate odoslať e-mail. Všimnite si podrobnú externú chybu, ktorá je k dispozícii v odrazovej správe. Podpora spoločnosti Microsoft vám možno nebude vedieť pomôcť ďalej.
