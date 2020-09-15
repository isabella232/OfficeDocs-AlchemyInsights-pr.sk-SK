---
title: Antispam – 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717340"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Riešenie problémov s doručovaním e-mailov s kódom chyby 5.7.23

Overte záznam SPF DNS pre svoju doménu na verejne dostupnej kontrole záznamov SPF alebo DNS na webe.

Overte, či výstupná správa nebola identifikovaná spoločnosťou Microsoft ako nevyžiadaná pošta, a smerovala cez [bazén s vysokým rizikom](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Správy v bazéne s vysokým rizikom neprejdú kontrolou SPF, a preto nebudú akceptované cieľovou e-mailovou organizáciou.

Ak problém pretrváva, možno bude potrebné obrátiť sa na správcu hostiteľa pošty, ku ktorému sa pokúšate Odoslať e-mail. Poznačte si podrobnú externú chybu dostupnú v správe Bounce. Technická podpora spoločnosti Microsoft nemusí byť schopná poskytnúť ďalšiu pomoc.
