---
title: Samoobslužný nákup prostredia PowerShell
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
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797736"
---
# <a name="self-service-purchase-of-powershell"></a>Samoobslužný nákup prostredia PowerShell

Ak chcete používať modul MSCommerce PowerShell, musíte ho nainštalovať do zariadenia s Windowsom 10 s TLS 1.2 (vyžadujú sa povolenia lokálneho správcu).  Importujte modul MSCommerce a pripojte sa k jeho modulu.  Po zobrazení výzvy na prihlásenie je potrebné použiť poverenia roly globálneho správcu alebo správcu fakturácie.  

Ak nemáte protokol TLS 1.2, pri pokuse o získanie alebo aktualizáciu politiky sa môže zobraziť nasledujúca chyba:

*ErrorMessage -Základné pripojenie sa zavrelo: Pri odosielaní sa vyskytla neočakávaná chyba.*



