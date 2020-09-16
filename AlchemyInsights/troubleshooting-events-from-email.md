---
title: Riešenie problémov s udalosťami z e-mailu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658749"
---
# <a name="troubleshooting-events-from-email"></a>Riešenie problémov s udalosťami z e-mailu

1. Overenie funkcie je povolená pre poštovú schránku: **Get-EventsFromEmailConfiguration- <mailbox> identity**

2. Potom sa pozrite na denníky udalostí z e-mailov **export-MailboxDiagnosticLogs <mailbox> -zložka TimeProfile**

3. V denníkoch udalostí z e-mailu vyhľadajte InternetMessageId, ktoré sa zhoduje s položkou v poštovej schránke.  

4. Vlastnosť TrustScore určuje, či sa položka pridá alebo nie. Udalosti sa pridajú iba v prípade, že TrustScore = "dôveryhodný".

TrustScore je určený vlastnosťami SPF, dkim alebo DMARC, ktoré sa nachádzajú v hlavičke správy.

Ak chcete zobraziť tieto vlastnosti:

**Počítačová verzia Outlooku**

- Otvorenie položky
- Súbor – > vlastnosti – > internetové hlavičky

alebo

**MFCMapi**

- Prechod na položku v priečinku Doručená pošta
- Vyhľadanie PR_TRANSPORT_MESSAGE_HEADERS_W

Tieto vlastnosti sa určia a zaznamenávajú počas prepravy a smerovania. Ďalšie riešenie problémov možno budete musieť spracovať prostredníctvom podpory prenosu informácií o zlyhaniach v SPF, DKIM a. alebo DMARC.