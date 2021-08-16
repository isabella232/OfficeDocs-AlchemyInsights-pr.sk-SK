---
title: Problémy s nárokmi a atribútmi tokenu
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012899"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problémy s nárokmi a atribútmi tokenu

**Aktualizácia, konfigurácia alebo odstránenie nárokov tokenov**

1. Pomocou služby Azure Active Directory (Azure AD) [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) môžete prispôsobiť typ nároku na uplatnenie nároku na rolu v tokene odpovede, ktorý dostanete po oprávnení aplikácie.
2. Vývojári aplikácií môžu vo svojich aplikáciách Azure AD použiť voliteľné nároky na určenie toho, ktoré nároky chcú v tokenoch odoslaných do ich aplikácie. Ďalšie informácie nájdete v téme [Poskytovanie voliteľných nárokov vo vašej aplikácii.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurácia skupinových nárokov na aplikácie pomocou Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ak sa vo vašej aplikácii používa bezproblémové jediné prihlásenie, pozrite si časť Prispôsobenie nárokov [vydaných v tokene SAML pre podnikové aplikácie.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Priradenie atribútov reklamácie**

1. Ak chcete konfigurovať politiku priraďovania nárokov pomocou prostredia PowerShell, pozrite si časť Prispôsobenie nárokov, ktoré sa vynechajú v rámci tokenov pre konkrétnu aplikáciu [v nájomníkovi (verzia Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Atribúty prípony schémy adresára poskytujú spôsob ukladania ďalších údajov vo Azure Active Directory objektoch používateľov a iných objektoch adresárov, ako sú napríklad skupiny, podrobnosti o nájomníkovi, hlavné mená služieb. Pri nárokoch na nároky na aplikácie možno v používateľských objektoch použiť iba rozšírené atribúty. [Použitie atribútov prípony adresára v nárokoch](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) popisuje, ako používať atribúty prípony adresára na odosielanie používateľských údajov do aplikácií v nárokoch tokenov.

Ďalšie informácie o nárokoch tokenov nájdete v téme:

- [Nároky v prístupových tokenoch](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Nároky v id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Nároky,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) ktoré môžete očakávať v ID tokenoch a prístupových tokenoch vydaných Azure AD B2C
- [Odkaz na nároky tokenu SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
