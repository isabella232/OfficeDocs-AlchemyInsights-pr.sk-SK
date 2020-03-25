---
title: Nie je možné prihlásiť sa do služby Teams z dôvodu chyby autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932290"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Nie je možné prihlásiť sa do služby Teams z dôvodu tejto autologon.microsoftazuread-sso dot com:443

Ak je v rámci overovania služby O365 zapnutá funkcia Seamless SSO, je možné, že je potrebné pridať URL adresu "autologon.microsoftazuread-sso.com" na intranetové lokality.  Ak sa už predtým pridala medzi dôveryhodné lokality a používa sa funkcia Seamless SSO, mala by sa odstrániť z dôveryhodných lokalít.

Prečítajte si [Kontrolný zoznam riešenia problémov s funkciou Seamless SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Ak chcete pridať URL adresu do zoznamu intranetových lokalít, postupujte podľa týchto krokov:

1. Otvorte Internet Explorer kliknutím na tlačidlo **Štart** Do vyhľadávacieho poľa zadajte text Internet Explorer a potom v zozname výsledkov kliknite na položku **Internet Explorer**.
2. Kliknite na položku **Nástroje** a potom kliknite na možnosť **Možnosti siete internet**.
3. Kliknite na kartu **Zabezpečenie**.
4. Teraz kliknite na položku **Lokálne intranetové lokality** a potom kliknite na tlačidlo **lokalít** a potom na tlačidlo **Rozšírené**.
5. Zadajte URL adresu webovej lokality a kliknite na položku **Pridať**.
6. Po dokončení nastavovania kliknite na tlačidlo **Zavrie5**.

Ďalšie informácie nájdete v téme [Dokumentácia pre nasadenie funkcie Seamless SSO pre službu O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (zahŕňa proces založený na zásadách na pridanie URL adresy na intranetové lokality v kroku 3).
