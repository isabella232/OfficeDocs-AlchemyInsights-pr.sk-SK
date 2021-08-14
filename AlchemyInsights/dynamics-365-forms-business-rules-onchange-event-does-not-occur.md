---
title: Obchodné pravidlá služby Dynamics 365 Forms – podnikové pravidlo, ktoré nie je odnímané pre formulár
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947314"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Udalosť PriZmene sa nevyskytuje, ak sa pole programovo zmení

Udalosť *PriZmene* sa nevyskytuje, ak sa pole pomocou atribútu zmení pomocou *programovania.* [nastaviť](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Metóduhodnoty. Ak chcete, aby sa obsluhy udalostí pre udalosť *PriZmene* spúšťali po nastavení hodnoty, musíte v kóde použiť atribút *formContext.data.entity* [fireOnchange.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
