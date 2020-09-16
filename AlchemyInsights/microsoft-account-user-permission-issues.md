---
title: Riešenie problému – používateľ sa nenašiel v adresári
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725422"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Riešenie problému – používateľ sa nenašiel v adresári

Ak sa používateľovi zobrazí chybové hlásenie "používateľ sa nenašiel" v adresári, skúste to znova, kde typ problému nie je používateľ v adresári.

Na vyriešenie problému je možné vykonať nasledujúce kroky.

- Uistite sa, že konto, ktoré prijalo e-mailovú pozvánku, je rovnaké ako konto, ktoré sa používa na prihlásenie neskôr. Uistite sa, že používateľ používa rovnaké konto na prijatie pozvania a prihlásenia na lokalitu. 

Ďalšie informácie nájdete v téme [spravovanie aliasov konta Microsoft </a> na spravovanie prihlásenia do služby Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Prejdite na všetky lokality, v ktorých sa používateľovi zobrazuje chyba. 

Pridajte text "/_layouts/15/People.aspx/MembershipGroupId = 0" (v rámci dvojitých úvodzoviek) na koniec URL adresy lokality. 

Príklad: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Vyberte používateľa v zozname.

- Na páse s nástrojmi kliknite na položku **odstrániť povolenia používateľa** . 
-  Pridajte späť používateľa a znova odošlite pozvánku používateľovi.

