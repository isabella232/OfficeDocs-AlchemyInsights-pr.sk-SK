---
title: 902 (chyby synchronizácie v dôsledku duplicitných objektov)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998809"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Chyby pri synchronizácii z dôvodu duplicitných objektov

Po dokončení synchronizácie adresárov v programe Outlook sa môže zobraziť niektoré z Microsoft 365:

- Nie je možné aktualizovať tento objekt v službách Microsoft Online Services, pretože nasledujúce atribúty priradené k tomuto objektu majú hodnoty, ktoré už môžu byť priradené k inému objektu v lokálnom adresári.

- Synchronizovaný objekt s rovnakou adresou servera proxy už existuje v adresári služieb Microsoft Online Services.

- Tento objekt nie je možné aktualizovať, pretože nasledujúce atribúty priradené k tomuto objektu majú hodnoty, ktoré už môžu byť priradené k inému objektu v lokálnych adresárových službách: UserPrincipalName.

Ak chcete identifikovať a opraviť problém, stiahnite a spustite nástroj Na opravu chýb [nástroja IdFix DirSync.](https://github.com/Microsoft/idfix)

Ďalšie informácie nájdete v téme [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
