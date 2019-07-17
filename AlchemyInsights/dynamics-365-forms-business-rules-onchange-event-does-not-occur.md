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
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748693"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="612fa-102">Udalosť OnChange sa nevyskytuje, ak pole sa zmenila programovo</span><span class="sxs-lookup"><span data-stu-id="612fa-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="612fa-103">Udalosť *OnChange* sa nevyskytuje, ak pole sa zmenila programovo pomocou *atribútu.* metóda [NastaviťHodnotu](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="612fa-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="612fa-104">Ak chcete obsluhy udalostí pre udalosti *OnChange* spustiť po nastavíte hodnotu musíte použiť *atribút formContext.data.entity.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) metóda v kóde.</span><span class="sxs-lookup"><span data-stu-id="612fa-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
