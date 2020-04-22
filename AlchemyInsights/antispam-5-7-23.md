---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676512"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Oprava problémov s doručením e-mailu pre kód chyby 5.7.23

Skontrolujte záznam SPF DNS pre vašu doménu na verejne dostupnej SPF alebo DNS záznam Checker na webe.

Overte, či odchádzajúca správa nebola identifikovaná ako spam spoločnosťou Microsoft a smerovaná cez [vysoko rizikové dodanie fondu](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Správy v bazéne s vysokým rizikom neprejdú SPF kontroly, a preto nebude prijatý cieľovej e-mailovej organizácie.

Ak problém pretrváva, možno budete musieť kontaktovať správcu poštového hostiteľa, ku ktorému sa pokúšate Odoslať e-mail. Poznačte si podrobnú externú chybu, ktorá je k dispozícii v správe o odskoku. Podpora spoločnosti Microsoft nemusí byť schopná pomôcť ďalej.
