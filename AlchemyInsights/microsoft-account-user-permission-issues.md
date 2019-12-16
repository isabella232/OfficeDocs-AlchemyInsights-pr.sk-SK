---
title: Riešenie problému-používateľ sa nenašiel v adresári
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054825"
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

