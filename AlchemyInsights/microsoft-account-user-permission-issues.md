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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754207"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Riešenie problému-používateľ sa nenašiel v adresári

Ak používatelia dostávajú chybové hlásenie "používateľ sa nenašiel" v adresári. Skúste to znova, ak je typ problému používateľ nie je v adresári.

Nasledujúce kroky môžu byť dokončené na vyriešenie problému.

- Uistite sa, že účet, ktorý prijal e-mailovú pozvánku je rovnaký účet, ktorý sa používa na prihlásenie neskôr. Uistite sa, že používateľ používa rovnaký účet prijať pozvanie a prihláste sa na lokalitu. 

Ďalšie informácie nájdete v téme [spravovanie aliasov konta</a> Microsoft na spravovanie prihlásenia na Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Prejdite na každú lokalitu, v ktorej používateľ dostane chybu. 

Pridať "/_layouts/15/People.aspx/MembershipGroupId = 0" (v úvodzovkách) na koniec adresy URL lokality. 

Príklad: https://_ lt_ "contoso">. SharePoint. com/_layouts/15/People. aspx/membershipGroupId = 0.

- Vyberte používateľa zo zoznamu.

- Kliknite na položku **odstrániť povolenia používateľa** z pása s nástrojmi. 
-  Pridajte späť používateľa a odošlite pozvánku používateľovi.

