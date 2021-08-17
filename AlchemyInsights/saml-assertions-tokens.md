---
title: SaML Assertions (Tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109255"
---
# <a name="saml-assertions-tokens"></a>SaML Assertions (Tokens)

1. Tokeny saML (Security Assertions Markup Language) sú vyjadrenia nárokov vo formáte XML. Tokeny SAML pre Windows Communication Foundation (WCF) sa predvolene používajú pri vydaných tokenoch federovaného zabezpečenia. Ďalšie informácie nájdete v téme [Tokeny a nároky SAML.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. Tieto Microsoft identity platform vyžarujú niekoľko typov tokenov zabezpečenia pri spracovaní každého toku overenia. [Odkaz na nároky tokenu SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) popisuje formát, vlastnosti zabezpečenia a obsah tokenov SAML 2.0.
3. Postupujte podľa pokynov v časti [Konfigurovateľné platnosti tokenov v Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) a porozumiete tomu, ako konfigurovať časy platnosti tokenov.
4. Postupujte podľa krokov uvedených v tomto [článku a porozumiete](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) tomu, ako nakonfigurovať šifrovanie tokenu Azure AD SAML.
5. V Azure AD môžete nastaviť možnosti podpisovania certifikátu a algoritmus podpisovania certifikátu. Ďalšie informácie nájdete v téme [Rozšírené možnosti podpisovania certifikátu v tokene SAML pre aplikácie galérie v Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)
