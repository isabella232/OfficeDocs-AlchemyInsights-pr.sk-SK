---
title: Tvrdenia SAML (tokeny)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885675"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="a7bd8-102">Tvrdenia SAML (tokeny)</span><span class="sxs-lookup"><span data-stu-id="a7bd8-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="a7bd8-103">Tokeny zabezpečenia tvrdení Markup Language (SAML) sú vyjadrenia XML pohľadávok.</span><span class="sxs-lookup"><span data-stu-id="a7bd8-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="a7bd8-104">Predvolene sa tokeny SAML tokeny Windows Communication Foundation (WCF) používajú v prípade externých bezpečnostných scenárov.</span><span class="sxs-lookup"><span data-stu-id="a7bd8-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="a7bd8-105">Ďalšie informácie nájdete v téme [tokeny SAML a reklamácie](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="a7bd8-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="a7bd8-106">Platforma Microsoft Identity emituje niekoľko typov tokenov zabezpečenia pri spracovaní každého toku overovania.</span><span class="sxs-lookup"><span data-stu-id="a7bd8-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="a7bd8-107">[Odkaz SAML tokeny](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) obsahuje popis formátu, charakteristík zabezpečenia a obsahu tokenov SAML 2,0.</span><span class="sxs-lookup"><span data-stu-id="a7bd8-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="a7bd8-108">Podľa pokynov v časti [konfigurovateľné tokeny životnosť v platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) sa naučíte, ako nakonfigurovať životnosť tokenov.</span><span class="sxs-lookup"><span data-stu-id="a7bd8-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="a7bd8-109">Postupujte podľa krokov uvedených v [tomto článku](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) a Pochopte, ako nakonfigurovať šifrovanie tokenu Azure AD SAML.</span><span class="sxs-lookup"><span data-stu-id="a7bd8-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="a7bd8-110">V službe Azure AD môžete nastaviť možnosti podpisu certifikátu a algoritmus podpisu certifikátu.</span><span class="sxs-lookup"><span data-stu-id="a7bd8-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="a7bd8-111">Ďalšie informácie nájdete v téme [Rozšírené možnosti podpisu certifikátu v tokene SAML pre aplikácie galérie v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="a7bd8-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
