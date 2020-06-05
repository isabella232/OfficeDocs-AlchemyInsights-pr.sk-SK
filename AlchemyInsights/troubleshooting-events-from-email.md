---
title: Riešenie problémov s udalosťami z e-mailu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569404"
---
# <a name="troubleshooting-events-from-email"></a>Riešenie problémov s udalosťami z e-mailu

1. Overte, či je zapnutá funkcia pre poštovú schránku: **Get-EventsFromEmailConfiguration -Identity <mailbox> **

2. Potom sa pozrite na "Udalosti z e-mailu" prihlási **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. V denníkoch "Udalosti z e-mailu" vyhľadajte InternetMessageId, ktorý zodpovedá položke v poštovej schránke.  

4. TrustScore určuje, či je položka pridaná alebo nie. Udalosti sa pridajú iba v prípade, že trustscore = "Dôveryhodný".

TrustScore je určený SPF, Dkim alebo Dmarc vlastnosti, ktoré sú v hlavičke správy.

Ak chcete zobraziť tieto vlastnosti:

**Výhľad na pracovnú plochu**

- Otvorenie položky
- Súbor -> Vlastnosti -> Internetové hlavičky

Alebo

**Mfcmapi**

- Prechod na položku v doručenej pošte
- Hľadajte PR_TRANSPORT_MESSAGE_HEADERS_W

Tieto vlastnosti sa určujú a zaznamenávajú počas prepravy a smerovania. Pre ďalšie riešenie problémov, budete musieť nadviazať s podporou prenosu o zlyhania sPF, DKIM a.alebo DMARC.