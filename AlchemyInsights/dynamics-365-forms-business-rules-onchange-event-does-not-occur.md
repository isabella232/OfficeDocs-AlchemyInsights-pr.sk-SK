---
title: Dynamics 365 tvorí Biznis pravidlá – pravidlo podnikania nie streľby pre formulár
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529034"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Udalosť OnChange sa nevyskytuje, ak pole sa zmenila programovo

Udalosť *OnChange* sa nevyskytuje, ak pole sa zmenila programovo pomocou *atribútu.* metóda [NastaviťHodnotu](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Ak chcete obsluhy udalostí pre udalosti *OnChange* spustiť po nastavíte hodnotu musíte použiť *atribút formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metóda v kóde.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
