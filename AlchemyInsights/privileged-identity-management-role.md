---
title: Privileged Identity Management roly
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973244"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management (PIM)

**Povolenia sa po aktivácii roly neudejú**

Keď aktivujete rolu v Azure AD Privileged Identity Management (PIM), aktivácia sa nemusí okamžite rozšíriť na všetky portály, ktoré vyžadujú privilegujúnú rolu. Niekedy sa môže zmena prejaviť aj po rozšírenie zmeny vo webovej vyrovnávacej autorite na portáli.

Ak je vaša aktivácia oneskorená, postupujte takto:

1. Odhláste sa z portálu Azure a potom sa znova prihláste. Po aktivácii roly služby Azure AD alebo roly zdroja v Azure sa vám zobrazí etapy aktivácie. Po dokončení všetkých etáp sa zobrazí prepojenie Odhlásiť sa. Na odhlásenie môžete použiť toto prepojenie. Vo väčšine prípadov sa tým vyrieši oneskorenie aktivácie.
2. V časti PIM overte, či ste uvedení ako člen roly.
3. Ak aktivujete rolu správcu Exchange, odhláste sa a znova sa prihláste. Ak problém pretrváva, otvorte žiadosť o podporu a zdvihnite ju ako problém. Ak používate rolu správcu Exchange na prístup do Centra zabezpečenia a dodržiavania súladu, pozrite si ďalší krok.
4. Ak aktivujete rolu na prístup do centra zabezpečenia a dodržiavania súladu alebo ak aktivujete rolu správcu služby SharePoint, môže sa vyskytnúť oneskorenie aktivácie v priebehu niekoľkých minút až niekoľkých hodín. Ide o známy problém a aktívne spolupracujeme s týmito tímami na čo možnom riešení tohto problému.

Ďalšie informácie nájdete v téme:

- [Aktivácia rolí služby Azure AD v PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Aktivácia rolí zdrojov v Azure v PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Po deaktivovaní roly alebo po uplynutí platnosti aktivácie roly sa povolenia neodstránia**

Po deaktivácii roly v službe Azure AD Privileged Identity Management alebo po uplynutí obdobia aktivácie roly môže byť oneskorenie, kedy budete mať prístup aj naďalej.

Ak sa deaktivácia oneskorí, postupujte takto:

1. Ak deaktivujete rolu správcu služby Exchange alebo uplynie obdobie aktivácie roly a všimnete si významné oneskorenie pred odstránením povolení, otvorte lístok technickej podpory a informujte svojho inžiniera technickej podpory, aby vám v rámci spoločnosti Office o tomto probléme pomohol vytvoriť lístok s tímom Privileged Access Management (PAM).
2. Ak uplynulo obdobie aktivácie, ale stále máte otvorenú reláciu prehliadača, zavrite prehliadač. Túto rolu môžete naďalej používať, kým túto reláciu nezatvoriť. Toto je známy problém a hľadáme potenciálnu opravu, ktorá má aktívne zrušiť každú reláciu po uplynutí platnosti aktivácie.

Ak sa oneskorenie líši od týchto dvoch scenárov, otvorte lístok technickej podpory.
