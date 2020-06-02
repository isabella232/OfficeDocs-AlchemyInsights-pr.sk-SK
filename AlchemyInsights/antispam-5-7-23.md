---
title: Antispam - 5.7.23
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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506458"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Riešenie problémov s doručovaním e-mailov s kódom chyby 5.7.23

Overte záznam DNS SPF pre svoju doménu pri verejne dostupnej kontrole záznamov SPF alebo DNS na webe.

Overte, či spoločnosť Microsoft neidentifikovala odchádzajúca správu ako nevyžiadanú poštu a smerovala cez [fond doručovania s vysokým rizikom.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Správy vo vysokorizikovom fonde doručovania neprejdú kontrolami SPF, a preto ich cieľová e-mailová organizácia neprijme.

Ak problém pretrváva, možno budete musieť kontaktovať správcu poštového hostiteľa, ktorému sa pokúšate odoslať e-mail. Poznačte si podrobnú externú chybu, ktorá je k dispozícii v správe o odskoku. Technická podpora spoločnosti Microsoft nemusí byť schopná ďalej pomáhať.
