---
title: Pripájanie k upozorneniam AAD
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037237"
---
# <a name="notification-aad-connect"></a>Pripájanie k upozorneniam AAD

- Uistite sa, že máte oprávnenie na vykonanie operácie. Globálni správcovia majú predvolene prístup. Okrem toho môžete použiť [riadenie prístupu na základe rolí](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) na delegovanie povolenia na registráciu prispievateľovi.
- Uistite sa, že sú povolené požadované koncové body a nie je blokovaný v dôsledku brány firewall. Podrobnosti nájdete v téme [požiadavky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registrácia môže zlyhať z dôvodu odchádzajúcej komunikácie, ktorá je podrobená kontrole SSL prostredníctvom sieťovej vrstvy.
- Skontrolujte, či ste overili nastavenie oznámení pre službu Azure AD Connect Health a skontrolujte nastavenie. Ak chcete zistiť, ako nakonfigurovať nastavenia oznámení pre oznámenia o stave pripojenia služby Azure AD, pozrite si túto [príručku](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Ak chcete získať ďalšie informácie o zostave synchronizácie so službou AAD Connect Health a o tom, ako si ju stiahnuť, pozrite si tému [synchronizácia na úrovni objektov](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Riešenie problémov s aplikáciou AAD Connect Health nájdete [v príručke na riešenie problémov s funkciou AAD pripojenie upozornení o stave údajov o zdraví](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) a v prípade najčastejšie kladených otázok sa nachádzajú v téme [bežné problémy pri inštalácii](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
