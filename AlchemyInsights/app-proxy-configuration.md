---
title: Konfigurácia servera proxy aplikácie
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885527"
---
# <a name="app-proxy-configuration"></a>Konfigurácia servera proxy aplikácie

1. Informácie o konfigurácii aplikácie proxy aplikácie v službe Azure AD na vystavenie lokálnych aplikácií do cloudu nájdete v téme Konfigurácia aplikácie [proxy aplikácie](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Jediné prihlásenie (SSO) umožňuje používateľom prístup k aplikácii bez overenia viackrát. Umožňuje vykonávať jednoduché overovanie v cloude v porovnaní so službou Azure Active Directory a umožňuje službe alebo spojnici zosobniť používateľa, aby dokončil akékoľvek ďalšie problémy s overovaním z aplikácie. Ďalšie informácie nájdete v téme [Konfigurácia jediného prihlásenia do aplikácie proxy aplikácie](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. [Tento článok](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) sa používa na riešenie bežných problémov, ktorým ľudia čelia pri vytváraní novej aplikácie proxy aplikácie.
4. Ak máte problém s nastavením záložnej autentifikácie v aplikácii, budete musieť riešiť problémy s [obmedzením delegovania delegovania Kerberos pre aplikačný Server](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) alebo sledovať pokyny týkajúce sa [konfigurácie aplikácie s PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) .
