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
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971354"
---
# <a name="user-provisioning"></a>Poskytovanie používateľov

- Použite funkciu [poskytovania na požiadanie](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) na poskytnutie používateľa a získanie podrobnej diagnostiky pre podnikaných krokov.
- Ak chcete riešiť problémy, ktoré sa vyskytnú pri poskytovaní služieb používateľom a skupinám, pozrite si príručku na riešenie problémov: [Nie sú k dispozícii používatelia.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Ak pozorujete, že používatelia sa nezriadujú, pozrite si článok [Poskytovanie denníkov (ukážka)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) v Azure Active Directory (AD). Vyhľadávať záznamy denníka týkajúce sa konkrétneho používateľa.
- Pravidelné reštartovanie poskytovania, aby ste zachytiť všetkých používateľov, ktorí sa zmeškali v predchádzajúcom cykle poskytovania.
- Používateľ alebo skupina možno nebola zhodnotená, pretože služba ešte nemá možnosť vyhodnotiť používateľa. Pozrite si pokyny na to, ako dlho trvá poskytovanie, ako aj indikátor priebehu na stránke konfigurácie poskytovania. Ak sa stabilný stav uvedený v časti Ďalšie podrobnosti nachádza pred dátumom vytvorenia/aktualizácie/odstránení používateľa, znamená to, že sme ešte nevyhodnocovali používateľa. V tomto scenári je najlepšie počkať, kým sa poskytovanie služby dokončí. Ak sa dosiahne stabilný stav, odporúčame vykonať reštart z používateľského rozhrania na portáli Azure.
  - Upozorňujeme, že naša služba vie len o zmenách používateľa alebo skupiny v zdrojovom systéme (Azure Active Directory). Ak sa používateľ alebo skupina odstráni priamo v aplikácii (napríklad ServiceNow), o týchto zmenách vieme a nevrátime ich späť na základe stavu používateľa v zdrojovom systéme. V tomto scenári je najlepšie vrátiť zmenu späť priamo v cieľovej aplikácii.
- Naša služba vyhodnotila používateľa alebo skupinu a zistila, že by sa nemala poskytnúť:
  - Ak ste rozsah nastavili tak, aby boli k aplikácii priradení používatelia a skupiny, skontrolujte, či je používateľ alebo skupina priradená k aplikácii.
  - Ak je používateľ alebo skupina priradená k aplikácii, uistite sa, že nie je priradená k predvolenej role prístupu. Túto rolu nie je možné použiť na poskytovanie.
  - Ak ste nastavili filter na určenie rozsahu na základe atribútov, uistite sa, že používateľ spĺňa zadané kritériá.
  - Ak už používatelia v cieľovom systéme existujú a stav používateľa v zdrojovom a cieľovom zhody, žiadne ďalšie kroky nevyberieme.
- Náš pokus o poskytnutie služby zlyhal a používateľ sa pokúsil o poskytnutie tejto služby. Pri týchto scenároch si pozrite kartu Riešenie problémov a odporúčania z denníkov poskytovania:
  - Požadovaný atribút používateľa môže v aplikácii Azure Active Directory chýbať alebo nezodpovedá formátu, ktorý vyžaduje aplikácia tretej strany. Atribút Krajina pre používateľa môže byť napríklad nastavený na hodnotu Spojené štáty, kedy by mal byť v USA.
  - Atribút je referenčný atribút, ktorý v cieľovej aplikácii ešte neexistuje. Referenčný atribút je atribút, ktorý odkazuje na iný objekt, napríklad používateľ, ktorý je členom skupiny. Identifikácia používateľa sa nachádza v atribúte člena skupiny, ale môže sa spracovať iba v prípade, že objekt používateľa, na ktorý odkazuje, už existuje.
