---
title: Riešenie problémov s udalosťami z e-mailu
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834854"
---
# <a name="troubleshooting-events-from-email"></a>Riešenie problémov s udalosťami z e-mailu

1. Overenie, či je funkcia pre poštovú schránku povolená: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Potom si pozrite denníky Udalosti z **e-mailu Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. V denníkoch Udalosti z e-mailu vyhľadajte InternetMessageId, ktorý sa zhoduje s položkou v poštovej schránke.  

4. Vlastnosť TrustScore určuje, či sa položka pridá alebo nie. Udalosti sa pridajú len vtedy, ak sa na hodnotu TrustScore = "Trusted" (Dôveryhodné).

Vlastnosť TrustScore určuje vlastnosti SPF, Dkim alebo Dmarc, ktoré sa nachádza v hlavičke správy.

Ak chcete zobraziť tieto vlastnosti:

**Počítačová aplikácia Outlook**

- Otvorenie položky
- File -> Properties -> Internet Headers

alebo

**MFCMapi**

- Prechod na položku v priečinku doručenej pošty
- Vyhľadajte PR_TRANSPORT_MESSAGE_HEADERS_W

Tieto vlastnosti sa určia a zaznamenajú počas prenosu a smerovania. Ak chcete vyriešiť ďalšie problémy, možno bude potrebné pokračovať s podporou prenosu v oblasti zlyhania pri SPF, DKIM a.alebo DMARC.