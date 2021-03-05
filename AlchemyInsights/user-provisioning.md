---
title: Poskytovanie používateľov
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
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482916"
---
# <a name="user-provisioning"></a>Poskytovanie používateľov

- Pomocou funkcie [na poskytovanie na požiadanie](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) môžete používateľovi poskytnúť podrobné informácie o vykonaných krokoch.
- Ak chcete riešiť problémy, s ktorými sa stretnete pri zriaďovaní používateľov a skupín, prečítajte si príručku na riešenie problémov, ktorá [sa neposkytuje používateľom](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Ak zistíte, že používatelia nie sú zriadení, pozrite si tému [poskytovanie denníkov (Preview)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) v službe Azure Active Directory (AD). Vyhľadajte položky denníka, ktoré súvisia s konkrétnym používateľom.
- Pravidelným reštartovaním poskytovania Zachyťte všetkých používateľov, ktorí zmeškali predchádzajúci cyklus poskytovania.
- Používateľ alebo skupina sa nemuseli poskytnúť, pretože naša služba ešte nemá možnosť hodnotenia používateľa. Pozrite si usmernenie o tom, ako dlho bude poskytovanie trvať, ako aj indikátor priebehu na stránke konfigurácie poskytovania. Ak je rovnovážny stav zadaný v časti Ďalšie podrobnosti pred dátumom vytvorenia/aktualizácie alebo odstránenia používateľa, znamená to, že sme zatiaľ nehodnotili používateľa. V tomto scenári je najvhodnejšie počkať na dokončenie poskytovania služby. Ak sa rovnovážny stav dosiahlo, odporúčame vám vykonať reštartovanie z používateľského rozhrania na portáli Azure.
  - Všimnite si, že naša služba je oboznámená len s zmenami používateľa alebo skupiny v zdrojovom systéme (Azure Active Directory). Ak sa používateľ alebo skupina odstráni priamo v aplikácii (napríklad ServiceNow), tieto zmeny nie sú známe a nie je možné ju vrátiť späť na základe stavu používateľa v zdrojovom systéme. V tomto scenári je najlepšie vrátiť zmeny priamo do cieľovej aplikácie.
- Naša služba hodnotila používateľa/skupinu a určila, že by sa nemala poskytovať:
  - Ak ste nastavili rozsah na priradených používateľov a skupiny, skontrolujte, či je používateľ alebo skupina priradená k aplikácii.
  - Ak je používateľ alebo skupina priradená k aplikácii, uistite sa, že nie je priradená k predvolenej úlohe prístupu. Túto rolu nie je možné použiť na poskytovanie.
  - Ak ste nastavili filter založený na atribútoch, overte, či používateľ spĺňa kritériá, ktoré ste zadali.
  - Ak už používatelia existujú v cieľovom systéme a stave používateľa v zdrojovej a cieľovej zhode, nebudeme mať žiadne ďalšie kroky.
- Služba sa pokúsila o poskytnutie používateľa a zlyhala. V prípade týchto scenárov si pozrite kartu Riešenie problémov a odporúčaní v denníkoch poskytovania:
  - Požadovaný atribút používateľa môže chýbať v službe Azure Active Directory alebo sa nezhoduje s formátom vyžadovaným aplikáciou tretej strany. Atribút krajiny na používateľa môže byť napríklad nastavený na Spojené štáty, Kedy by mal byť v USA.
  - Atribút je referenčný atribút, ktorý ešte neexistuje v cieľovej aplikácii. Referenčný atribút je atribút, ktorý odkazuje na iný objekt, napríklad na používateľa, ktorý je členom skupiny. ID používateľa bude v atribúte člena skupiny, ale môže sa spracovať iba v prípade, že objekt používateľa odkazuje na už existuje.
