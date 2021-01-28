---
title: Problémy s pohľadávkami a atribútmi tokenu
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035972"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problémy s pohľadávkami a atribútmi tokenu

**Aktualizácia, konfigurovanie alebo odstránenie tokenov pohľadávok**

1. Pomocou služby Azure Active Directory (Azure AD) môžete [prispôsobiť typ deklarácie pre nárok na rolu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) v tokene odpovede, ktorý dostanete po povolení aplikácie.
2. Vývojári aplikácií môžu vo svojich aplikáciách Azure AD použiť voliteľné nároky na určenie tvrdení, ktoré chcú v tokenoch odoslaných do ich aplikácie. Ďalšie informácie nájdete v téme [poskytovanie voliteľných nárokov v aplikácii](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Konfigurácia skupinových pohľadávok pre aplikácie so službou Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ak používate bezproblémové jediné prihlásenie v aplikácii, pozrite si tému [Prispôsobenie pohľadávok vydaných v tokene SAML pre podnikové aplikácie](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Priradenie atribútov pohľadávok**

1. Ak chcete konfigurovať politiku priradenia pohľadávok pomocou prostredia PowerShell, pozrite si tému [Prispôsobenie pohľadávok emitovaných tokenmi pre konkrétnu aplikáciu v nájomníkovi (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Atribúty prípony adresárovej schémy poskytujú spôsob ukladania ďalších údajov v službe Azure Active Directory na objekty používateľa a iné objekty adresárov, ako sú napríklad skupiny, Podrobnosti o nájomníkovi, princípy služby. Na vyžarovanie pohľadávok do aplikácií sa môžu použiť len atribúty prípony na používateľských objektoch. [Používanie atribútov prípony v adresárových schémach v žiadostiach](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) popisuje, ako používať atribúty prípony adresárovej schémy na odosielanie používateľských údajov do aplikácií v tokenových pohľadávkach.

Ďalšie informácie o tokenových pohľadávkach nájdete v témach:

- [Pohľadávky v accessových tokenoch](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Nároky v id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Požiadavky](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , ktoré možno očakávať v tokenoch identifikácie a prístupových tokenoch vydaných službou Azure AD B2C
- [Odkaz na deklaráciu SAML tokenu](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
