---
title: Problém so stavom služby AAD Pripojenie AAD
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923767"
---
# <a name="problem-with-aad-connect-health"></a>Problém so stavom služby AAD Pripojenie AAD

- Uistite sa, že máte oprávnenie vykonávať operáciu. Globálni správcovia majú predvolene prístup. Okrem toho môžete použiť prístupový ovládací [prvok založený na rolách na](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) delegovanie registračného povolenia prispievateľa.
- Zabezpečte, aby boli požadované koncové body povolené a nie sú blokované pre bránu firewall. Podrobnosti nájdete v časti [požiadavky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registrácia môže zlyhať z dôvodu odchádzajúcej komunikácie, ktorá je podrobená kontrole SSL prostredníctvom sieťovej vrstvy.
- Skontrolujte nastavenia oznámení služby Azure AD Pripojenie Stav. Skontrolujte svoje nastavenie. Táto [príručka](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vám pomôže pochopiť, ako konfigurovať nastavenia oznámení pre oznámenia o stave služby Azure AD Pripojenie oznámenia o stave.
- Ďalšie informácie o zostave synchronizácie služby AAD Pripojenie Health a o tom, ako ju stiahnuť, nájdete v téme Správa o [synchronizácii na úrovni objektov.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Ak chcete riešiť problémy Pripojenie upozornení služby AAD pre stav, postupujte podľa príručky na riešenie problémov s upozorneniami na stav služby [AAD Pripojenie a](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) v prípade bežných otázok si pozrite tému Bežné otázky týkajúce sa inštalácie služby [AAD Pripojenie Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
