---
title: Riešenie problémov – používateľ sa nenašiel v adresári
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098185"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Riešenie problémov – používateľ sa nenašiel v adresári

Ak sa používateľom zobrazuje chybové hlásenie Používateľ sa v adresári nedá nájsť, skúste to znova, ak sa v adresári nachádza možnosť Typ problému Používateľ.

Na vyriešenie problému možno vykonať tieto kroky.

- Skontrolujte, či je konto, ktoré prijalo e-mailovú pozvánku, rovnaké ako konto, ktoré sa používa na prihlásenie neskôr. Skontrolujte, či používateľ používa rovnaké konto na prijatie pozvánky a prihlásenie na lokalitu. 

Ďalšie informácie nájdete v [téme Spravovanie aliasov konta Microsoft </a> na spravovanie Microsoft 365 prihlásenia](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Prejdite na všetky lokality, v ktorých sa používateľovi zobrazuje chyba. 

Na koniec URL adresy lokality pridajte "/_layouts/15/people.aspx/membershipgroupid=0" (v dvojitých úvodzovkách). 

Príklad: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- V zozname vyberte používateľa.

- Na **páse s nástrojmi kliknite** na položku Odstrániť povolenia používateľov. 
-  Pridajte používateľa späť a znova odoslať pozvánku používateľovi.

