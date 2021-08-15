---
title: Problém s jedným používateľom
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960166"
---
# <a name="problem-with-single-user"></a>Problém s jedným používateľom

- Používateľ možno nebol zverejnený, pretože služba ešte nemá možnosť vyhodnotiť používateľa. Pozrite si pokyny na to, ako dlho trvá poskytovanie, ako aj indikátor priebehu na stránke konfigurácie poskytovania. Ak sa stabilný stav uvedený v časti Ďalšie podrobnosti nachádza pred dátumom vytvorenia/aktualizácie/odstránení používateľa, znamená to, že sme ešte nevyhodnocovali používateľa. V tomto scenári je najlepšie počkať, kým sa poskytovanie služby dokončí.

  - Upozorňujeme, že naša služba vie len o zmenách používateľa v zdrojovom systéme (Cloud HR). Ak chcete zistiť zmenu a tok tejto zmeny do služby Active Directory, v zdrojovom systéme služby Azure AD sa musí nachádzať platná zmena.
- Poskytovanie služby vyhodnotilo používateľa a určilo, že by sa nemala poskytnúť:
  - Ak ste nastavili filter na určenie rozsahu na základe atribútov, uistite sa, že používateľ spĺňa zadané kritériá.
  - Ak už používatelia v cieľovom systéme existujú a stav používateľa v zdrojovom a cieľovom zhody, žiadne ďalšie kroky nevyberieme.
- Poskytovanie služby sa pokúsilo poskytnúť používateľovi, čo zlyhalo. Pri týchto scenároch si pozrite kartu Riešenie problémov a odporúčania z denníkov poskytovania:
  - V lokálnej službe Active Directory alebo Azure AD môže chýbať požadovaný atribút používateľa. Pravidlá generácie userPrincipalName alebo sAMAccountName napríklad negenerujú správnu hodnotu.
  - Priraďovací atribút (zvyčajne employeeId) sa neodporúča vyriešiť pre jedinečného používateľa v lokálnej službe Active Directory alebo Azure AD. Existujú napríklad dvaja používatelia s rovnakým id zamestnanca v AD a služba vráti kód chyby, ktorý označuje duplicitné cieľové položky pre rovnakú položku zdroja.

Ak chcete skontrolovať denníky jedného používateľa a skupín, pozrite si tému Kontrola denníkov [poskytovania pre problém konkrétneho používateľa.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
