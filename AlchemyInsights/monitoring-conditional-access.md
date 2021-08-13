---
title: Monitorovanie podmieneného prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975116"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorovanie podmieneného prístupu pre Exchange

Ak používatelia zameraní na podmienený prístup nespĺňajú požiadavky vašej organizácie na prístup, dostanú e-mailové oznámenie. Na vyriešenie tohto problému odporúčame jedno alebo viacero z nasledujúcich riešení:

- Ak by malo byť zariadenia zaregistrované, poraďte používateľovi, aby Company Portal aplikácie a overil, či sa zariadenie zobrazí v Company Portal. Ak sa tak stane, používateľ by mal zariadenie zaregistrovať.
- Na portáli Azure prejdite na položku Intune > Súlad zariadení. V časti Monitorovať kliknite na položku Súlad zariadení. Pozrite si hlásenie o dodržiavaní súladu zariadenia a overte, či je zariadenie používateľa označené ako kompatibilné.
- Na portáli Azure prejdite na položku Intune > Súlad zariadení. V časti Správa kliknite na položku Politiky. V zozname politík dodržiavania súladu overte, či je k zariadeniu používateľa priradený profil. Ak nie je priradený žiadny profil, služba Intune nebude môcť potvrdiť súlad zariadenia.
- Upravte priradenie podmieneného prístupu používateľa.

1. Na portáli Azure prejdite na službu **Intune**  >  **– politiky podmieneného**  >  **prístupu.**
2. Vyberte politiku zo zoznamu.
3. Kliknite na položku Používatelia a skupiny.
4. Ak chcete na niekoho zacieliť určitú politiku, pridajte ho do zoznamu Zahrnúť. Ak chcete zabezpečiť, aby sa osoba v politike nezanechá, pridajte ju do zoznamu Vylúčiť.

Užitočné prepojenia:

[Prehľad súladu zariadení](https://docs.microsoft.com/intune/device-compliance-get-started)

[Riešenie problémov s certifikačnou autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Politika riešenia problémov](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorovanie dodržiavania súladu zariadení so intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Poznámka: Tieto kroky sú užitočné len pri riešení problémov Azure Active Directory podmieneného prístupu. K dispozícii je tiež možnosť umiestniť do karantény prístup zariadenia blokujúcemu e-mail s Exchange politiky. Ďalšie informácie o Exchange zariadení nájdete na stránke [tu]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
