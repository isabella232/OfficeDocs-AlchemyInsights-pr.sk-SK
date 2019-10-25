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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682286"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Oprava problémov s doručením e-mailu pre kód chyby 5.7.23

Skontrolujte záznam SPF DNS pre vašu doménu na verejne dostupnej SPF alebo DNS záznam Checker na webe.

Overte, či odchádzajúca správa nebola identifikovaná ako spam v balíku Office 365 a smerovaný cez [vysoko rizikové dodanie fondu](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Správy v bazéne s vysokým rizikom neprejdú SPF kontroly, a preto nebude prijatý cieľovej e-mailovej organizácie.

Ak problém pretrváva, možno budete musieť kontaktovať správcu poštového hostiteľa, ku ktorému sa pokúšate Odoslať e-mail. Poznačte si podrobnú externú chybu, ktorá je k dispozícii v správe o odskoku.  Podpora balíka Office 365 nemusí byť schopná pomôcť ďalej.