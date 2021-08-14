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
ms.openlocfilehash: a187fec34ef3eae485a8a880127b5f82a028edb7f0e9a276a41b5e33cad25ead
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942850"
---
# <a name="self-service-purchase-of-powershell"></a>Samoobslužný nákup prostredia PowerShell

Ak chcete používať modul MSCommerce PowerShell, musíte ho nainštalovať do Windows 10 zariadenia s TLS 1.2 (vyžadujú sa povolenia lokálneho správcu).  Importujte modul MSCommerce a pripojte sa k jeho modulu.  Po zobrazení výzvy na prihlásenie je potrebné použiť poverenia roly globálneho správcu alebo správcu fakturácie.  

Ak nemáte protokol TLS 1.2, pri pokuse o získanie alebo aktualizáciu politiky sa môže zobraziť nasledujúca chyba:

*ErrorMessage -Základné pripojenie sa zavrelo: Pri odosielaní sa vyskytla neočakávaná chyba.*



