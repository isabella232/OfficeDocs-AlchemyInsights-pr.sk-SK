---
title: Konfigurácia proxy aplikácie
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
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951580"
---
# <a name="app-proxy-configuration"></a>Konfigurácia proxy aplikácie

1. Ak chcete zistiť, ako nakonfigurovať aplikáciu proxy aplikácie v Azure AD, aby sa vaše lokálne aplikácie vystavili do cloudu, pozrite si časť Konfigurácia [aplikácie proxy aplikácie.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Jediné prihlásenie (SSO) umožňuje používateľom prístup k aplikácii bez viacnásobného overenia. Umožňuje, aby sa jediné overovanie v cloude vyskytol v prípade spoločnosti Azure Active Directory a umožňuje službe alebo konektoru zosobnenie používateľa, aby v aplikácii dokončili akékoľvek ďalšie výzvy overovania. Ďalšie informácie nájdete v téme [Konfigurácia jediného prihlásenia do aplikácie proxy aplikácie.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Tento [článok vám umožňuje](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) riešiť bežné problémy, s ktoré ľudia pri vytváraní novej aplikácie proxy aplikácie predídu.
4. Ak máte problém s nastavením serverové overovanie v aplikácii, možno budete musieť vyriešiť problém s konfiguráciou delegovania s obmedzenou protokolom [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) pre aplikačný server proxy alebo postupujte podľa pokynov na konfiguráciu aplikácie so službou [PingAccess,](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) aby sa váš problém vyriešil.
