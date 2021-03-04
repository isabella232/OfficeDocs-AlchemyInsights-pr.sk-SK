---
title: Problém s jediným používateľom
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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430206"
---
# <a name="problem-with-single-user"></a>Problém s jediným používateľom

- Používateľ nemusí byť zriadený, pretože služba ešte nemá možnosť hodnotenia používateľa. Pozrite si usmernenie o tom, ako dlho bude poskytovanie trvať, ako aj indikátor priebehu na stránke konfigurácie poskytovania. Ak je rovnovážny stav zadaný v časti Ďalšie podrobnosti pred dátumom vytvorenia/aktualizácie alebo odstránenia používateľa, znamená to, že sme zatiaľ nehodnotili používateľa. V tomto scenári je najvhodnejšie počkať na dokončenie poskytovania služby.

  - Všimnite si, že naša služba je oboznámená len s zmenami používateľa v zdrojovom systéme (cloud HR). Pri zisťovaní zmeny a jeho toku do služby Active Directory musí byť platná zmena v zdrojovom systéme pre Azure AD.
- Poskytovanie služby vyhodnotilo používateľa a určilo sa, že by sa nemalo poskytovať:
  - Ak ste nastavili filter založený na atribútoch, overte, či používateľ spĺňa kritériá, ktoré ste zadali.
  - Ak už používatelia existujú v cieľovom systéme a stave používateľa v zdrojovej a cieľovej zhode, nebudeme mať žiadne ďalšie kroky.
- Poskytovanie služby sa pokúsilo o poskytnutie používateľa a zlyhalo. V prípade týchto scenárov si pozrite kartu Riešenie problémov a odporúčaní v denníkoch poskytovania:
  - V lokálnej službe Active Directory alebo službe Azure AD môže chýbať požadovaný atribút používateľa. Pravidlá tvorby userPrincipalName alebo sAMAccountName napríklad nevytvárajú správnu hodnotu.
  - Zodpovedajúci atribút (zvyčajne klíč) sa nerieši jedinečnému používateľovi v lokálnej službe Active Directory alebo v službe Azure AD. Napríklad existujú dvaja používatelia s rovnakým klíč v REKLAMe a služba vráti kód chyby označujúci duplicitné cieľové položky pre tú istú zdrojovú položku.

Ak chcete skontrolovať denníky pre jedného používateľa a skupiny, pozrite si tému [Revízia denníkov poskytovania problému s konkrétnym používateľom](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
