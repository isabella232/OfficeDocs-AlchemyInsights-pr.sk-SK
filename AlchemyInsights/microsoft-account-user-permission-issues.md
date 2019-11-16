---
title: Riešenie problému-používateľ sa nenašiel v adresári
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768816"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Riešenie problému-používateľ sa nenašiel v adresári

Ak používatelia dostávajú chybové hlásenie "používateľ sa nenašiel" v adresári, skúste to znova, ak je typ problému používateľ nie je v adresári.

Nasledujúce kroky môžu byť dokončené na vyriešenie problému.

- Uistite sa, že účet, ktorý prijal e-mailovú pozvánku je rovnaký účet, ktorý sa používa na prihlásenie neskôr. Uistite sa, že používateľ používa rovnaký účet prijať pozvanie a prihláste sa na lokalitu. 

Ďalšie informácie nájdete v téme [spravovanie aliasov konta</a> Microsoft na spravovanie prihlásenia na Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Prejdite na každú lokalitu, v ktorej používateľ dostane chybu. 

Pridať "/_layouts/15/People.aspx/MembershipGroupId = 0" (v úvodzovkách) na koniec adresy URL lokality. 

Príklad: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Vyberte používateľa zo zoznamu.

- Kliknite na položku **odstrániť povolenia používateľa** z pása s nástrojmi. 
-  Pridajte späť používateľa a odošlite pozvánku používateľovi.

