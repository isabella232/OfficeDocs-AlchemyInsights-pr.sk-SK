---
title: Nie je možné prihlásiť sa do služby Teams z dôvodu chyby autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038415"
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
