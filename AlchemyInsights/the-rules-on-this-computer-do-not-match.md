---
title: 'Chyba: pravidlá v tomto počítači sa nezhodujú'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690978"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Chyba: pravidlá v tomto počítači sa nezhodujú

Ak chcete zobraziť aktualizovaný stav tohto známeho problému, pozrite si tému [pravidlá v tomto počítači sa nezhodujú s pravidlami na serveri Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Tím Outlooku implementoval opravu v zostave 12928,10000. Oprava je už na lokalite Insider Fast a prechod na mesačný kanál sa koncom júna 2020. Po vytvorení pevnej zostavy sa môže zobraziť výzva "ktoré pravidlá si chcete ponechať" naposledy. Po zobrazení výzvy vyberte položku Server a potom sa vráťte späť v Outlooku a znova zapnite všetky pravidlá, ktoré boli vypnuté.

Kým nie je k dispozícii oprava, použite toto alternatívne riešenie:

**Alternatívne riešenie**: v nedávnych zostavách sa vyskytol problém pre tých, ktorí vytvorili len pravidlá klienta v počítačovej verzii Outlooku. Ak sa problém vyskytuje aj naďalej, zvážte odstránenie pravidiel a potom vytváranie a úprava pravidiel len v aplikácii OWA (Outlook Web App) dovtedy, kým sa problém nevyrieši.

Ak nemôžete odstrániť pravidlá manuálne môžete spustiť Outlook príkaz pri spustení Outlooku spustením Outlook.exe/Cleanrules. Týmto sa odstránia pravidlá klienta aj servera. Odstránia sa všetky pravidlá pre všetky kontá v profile programu Outlook. Tento príkaz je ďalej zdokumentovaný v článku prepínače príkazového tlačidla.

