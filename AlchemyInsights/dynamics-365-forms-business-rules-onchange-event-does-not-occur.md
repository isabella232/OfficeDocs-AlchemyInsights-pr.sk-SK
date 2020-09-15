---
title: Dynamics 365 formuláre obchodné pravidlá – pravidlo podnikania nie je vypaľovanie formulára
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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711506"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>Prizmene udalosť sa nevyskytne, ak sa pole zmení pomocou programovania

Udalosť *prizmene* sa nevyskytne, ak sa pole zmení pomocou programovania pomocou *atribútu.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metóda. Ak chcete, aby sa obsluha udalostí pre udalosť *prizmene* spustila po nastavení hodnoty, musíte v kóde použiť metódu *formContext. Data. entity* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) .

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
