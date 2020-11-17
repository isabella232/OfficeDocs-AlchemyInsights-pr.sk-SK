---
title: Rola s privilegovaným správaním identity
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089152"
---
# <a name="privileged-identity-managementpim-role"></a>Rola správy privilegovaných identít (PIM)

**Povolenia sa neudelia po aktivácii roly**

Pri aktivácii roly v službe Azure AD privileged Identity Management (PIM) sa aktivácia nemusí okamžite rozšíriť na všetky portály, ktoré vyžadujú privilegovanú rolu. Niekedy aj v prípade, že sa zmena rozšírila, web caching na portáli môže mať za následok zmeny, ktoré sa neprejavia okamžite.

Ak je vaša Aktivácia oneskorená, postupujte podľa týchto krokov:

1. Odhláste sa zo služby Azure Portal a potom sa znova prihláste. Keď aktivujete rolu Azure AD alebo rolu Azure Resource, zobrazia sa vám fázy aktivácie. Po dokončení všetkých fáz sa zobrazí prepojenie odhlásiť sa. Ak sa chcete odhlásiť, môžete použiť toto prepojenie. Tým sa vyrieši väčšina prípadov oneskorenia aktivácie.
2. V PIM Skontrolujte, či ste ako člen roly zaradení.
3. Ak aktivujete rolu správcu servera Exchange, skontrolujte, či sa odhlásite a znova prihlásite. Ak problém pretrváva, otvorte lístok technickej podpory a Vyzdvihnite ho ako problém. Ak používate rolu správcu servera Exchange na prístup k centru zabezpečenia a dodržiavania súladu, pozrite si ďalší krok.
4. Ak aktivujete rolu na prístup k centru zabezpečenia a dodržiavania súladu, alebo Ak aktivujete rolu správcu služby SharePoint, niektoré oneskorené aktivácie sa vyskytnú od niekoľkých minút až do niekoľkých hodín. Toto je známy problém a aktívne pracujeme s týmito tímami na vyriešenie tohto problému čo najskôr.

Ďalšie informácie nájdete v téme:

- [Aktivácia rol služby Azure AD v PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivácia rolí Azure Resource v PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Povolenia sa neodstránia po deaktivácii roly alebo po uplynutí platnosti aktivácie roly**

Keď deaktivujete rolu v službe Azure AD privilegovaná správa identít alebo po uplynutí obdobia aktivácie roly, môže sa stať, že budete mať naďalej prístup.

Ak sa deaktivácia oneskorí, postupujte podľa týchto krokov:

1. Ak deaktivujete rolu správcu servera Exchange alebo uplynie obdobie aktivácie roly a zistíte, že pred odstránením povolení uplynulo značné oneskorenie, otvorte lístok technickej podpory a informujte svojho pracovníka technickej podpory, aby vám pomohol pomenovať letenku s tímom PAM (privilegovaný prístup Management) v rámci balíka Office o tomto probléme.
2. Ak uplynula platnosť obdobia aktivácie, ale stále máte otvorenú reláciu prehliadača, ukončite prehliadač. Rolu môžete naďalej používať, až kým nezavriete danú reláciu. Ide o známy problém a my sa pozrieme na možnú opravu, aby ste po uplynutí platnosti aktivácie aktívne zrušili každú reláciu.

Ak je oneskorenie iné ako tieto dva scenáre, otvorte lístok technickej podpory.
