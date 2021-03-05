---
title: Problém s funkciou AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483119"
---
# <a name="problem-with-aad-connect-health"></a>Problém s funkciou AAD Connect Health

- Uistite sa, že máte oprávnenie na vykonanie operácie. Globálni správcovia majú predvolene prístup. Okrem toho môžete použiť [riadenie prístupu na základe rolí](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) na delegovanie povolenia na registráciu prispievateľovi.
- Uistite sa, že sú povolené požadované koncové body a nie je blokovaný v dôsledku brány firewall. Podrobnosti nájdete v téme [požiadavky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registrácia môže zlyhať z dôvodu odchádzajúcej komunikácie, ktorá je podrobená kontrole SSL prostredníctvom sieťovej vrstvy.
- Skontrolujte, či ste overili nastavenie oznámení v službe Azure AD Connect Health. Skontrolujte nastavenie. Táto [príručka](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vám pomôže pochopiť, ako nakonfigurovať nastavenia oznámení pre oznámenia o stave pripojenia služby Azure AD.
- Ak chcete získať ďalšie informácie o zostave synchronizácie so službou AAD Connect Health a o tom, ako si ju stiahnuť, pozrite si tému [synchronizácia na úrovni objektov](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Ak chcete riešiť problémy so zobrazovaním upozornení o stave pripojenia AAD, postupujte podľa pokynov na [Riešenie problémov s funkciou AAD pripojenie upozornení o stave údajov o zdraví](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) a v prípade najčastejšie kladených otázok nájdete v téme [bežné problémy so stavom inštalácie](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
