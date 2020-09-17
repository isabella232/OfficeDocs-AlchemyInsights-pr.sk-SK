---
title: Kód chyby 550 5.7.501 prístup odmietnutý, zistené zneužitie nevyžiadanej pošty
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784070"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a>550 5.7.501 prístup odmietnutý, zistené zneužitie nevyžiadanej pošty

Táto správa sa zvyčajne vyskytuje vtedy, keď používatelia odosielajú e-mailové správy z IP adries pomocou domény Initial *. onmicrosoft.com* , ktorá je priradená novým nájomníkom v Microsoft 365. Najjednoduchším spôsobom, ako tento problém vyriešiť, je:

1. [Pridajte doménu do nájomníka](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).

2. [Zmeňte primárnu e-mailovú adresu používateľov](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) na novú vlastnú doménu, ktorú ste práve pridali.
