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
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769354"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="c82da-102">Udalosť OnChange nenastane, ak sa pole zmení programovo</span><span class="sxs-lookup"><span data-stu-id="c82da-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="c82da-103">Udalosť *onChange* nenastane, ak sa pole zmení programovo pomocou *atribútu.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metóda.</span><span class="sxs-lookup"><span data-stu-id="c82da-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="c82da-104">Ak chcete obsluhy udalostí pre udalosť *onChange* spustiť po nastavíte hodnotu musíte použiť *formcontext. Data. entity atribút* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metóda vo vašom kóde.</span><span class="sxs-lookup"><span data-stu-id="c82da-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
