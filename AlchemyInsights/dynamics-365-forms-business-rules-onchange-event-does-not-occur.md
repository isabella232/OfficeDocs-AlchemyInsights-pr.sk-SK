---
title: Dynamics 365 formuláre obchodné pravidlá-obchodné pravidlo nie je paľba pre formulár
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529034"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Udalosť OnChange nenastane, ak sa pole zmení programovo

Udalosť *onChange* nenastane, ak sa pole zmení programovo pomocou *atribútu.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metóda. Ak chcete obsluhy udalostí pre udalosť *onChange* spustiť po nastavíte hodnotu musíte použiť *atribút formcontext. Data. entity.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metóda vo vašom kóde.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
