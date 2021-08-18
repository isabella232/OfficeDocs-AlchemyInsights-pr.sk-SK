---
title: Monitorovanie podmieneného prístupu v Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327572"
---
# <a name="monitor-intune-conditional-access"></a>Monitorovanie podmieneného prístupu v Intune

Ak používatelia zameraní na podmienený prístup nespĺňajú požiadavky vašej organizácie na prístup, dostanú e-mailové oznámenie. Na vyriešenie tohto problému odporúčame jedno alebo viacero z nasledujúcich riešení:

1. Ak by malo byť zariadenia zaregistrované, poraďte používateľovi, aby Company Portal aplikácie a overil, či sa zariadenie zobrazí v Company Portal. Ak sa tak stane, používateľ musí zariadenie zaregistrovať.
1. Na portáli Azure prejdite na do **časti Súlad zariadení so službou Intune.**  >   
1. Ak chcete zobraziť hlásenie o dodržiavaní súladu zariadenia a overiť, či je zariadenie kompatibilné, kliknite v časti **Monitor** na položku Súlad **zariadení.**
1. Na portáli Azure prejdite na do **časti Súlad zariadení so službou Intune.**  >   V **časti Správa kliknite** na položku **Politiky**. V zozname politík dodržiavania súladu overte, či je k zariadeniu používateľa priradený profil. Ak nie je priradený žiadny profil, služba Intune nebude môcť potvrdiť súlad zariadenia.
1. Upravte priradenie podmieneného prístupu používateľa.
1. Na portáli Azure prejdite na položku Politiky podmieneného prístupu služby **Intune,** vyberte politiku zo zoznamu  >    >  a kliknite na položku **Používatelia a skupiny**.
1. Ak chcete na niekoho zacieliť určitú politiku, pridajte ho do **zoznamu Zahrnúť.** Ak chcete zabezpečiť, aby sa osoba v politike nezanechá, pridajte ju do **zoznamu Vylúčiť.**

**Užitočné prepojenia:**

- [Prehľad súladu zariadení](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Riešenie problémov s certifikačnou autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Politika riešenia problémov](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorovanie dodržiavania súladu zariadení so intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Poznámka:** Tieto kroky sú užitočné len pri riešení problémov Azure Active Directory s podmieneným prístupom. Zo zariadenia, ktoré blokuje prístup k e-mailu, možno umiestniť do karantény aj s Exchange politiky. Ďalšie informácie o Exchange zariadení nájdete [**tu.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
