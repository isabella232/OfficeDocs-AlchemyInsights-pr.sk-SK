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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="5cc23-102">Problémy s pohľadávkami a atribútmi tokenu</span><span class="sxs-lookup"><span data-stu-id="5cc23-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="5cc23-103">**Aktualizácia, konfigurovanie alebo odstránenie tokenov pohľadávok**</span><span class="sxs-lookup"><span data-stu-id="5cc23-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="5cc23-104">Pomocou služby Azure Active Directory (Azure AD) môžete [prispôsobiť typ deklarácie pre nárok na rolu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) v tokene odpovede, ktorý dostanete po povolení aplikácie.</span><span class="sxs-lookup"><span data-stu-id="5cc23-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="5cc23-105">Vývojári aplikácií môžu vo svojich aplikáciách Azure AD použiť voliteľné nároky na určenie tvrdení, ktoré chcú v tokenoch odoslaných do ich aplikácie.</span><span class="sxs-lookup"><span data-stu-id="5cc23-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="5cc23-106">Ďalšie informácie nájdete v téme [poskytovanie voliteľných nárokov v aplikácii](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="5cc23-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="5cc23-107">[Konfigurácia skupinových pohľadávok pre aplikácie so službou Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="5cc23-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="5cc23-108">Ak používate bezproblémové jediné prihlásenie v aplikácii, pozrite si tému [Prispôsobenie pohľadávok vydaných v tokene SAML pre podnikové aplikácie](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="5cc23-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="5cc23-109">**Priradenie atribútov pohľadávok**</span><span class="sxs-lookup"><span data-stu-id="5cc23-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="5cc23-110">Ak chcete konfigurovať politiku priradenia pohľadávok pomocou prostredia PowerShell, pozrite si tému [Prispôsobenie pohľadávok emitovaných tokenmi pre konkrétnu aplikáciu v nájomníkovi (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="5cc23-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="5cc23-111">Atribúty prípony adresárovej schémy poskytujú spôsob ukladania ďalších údajov v službe Azure Active Directory na objekty používateľa a iné objekty adresárov, ako sú napríklad skupiny, Podrobnosti o nájomníkovi, princípy služby.</span><span class="sxs-lookup"><span data-stu-id="5cc23-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="5cc23-112">Na vyžarovanie pohľadávok do aplikácií sa môžu použiť len atribúty prípony na používateľských objektoch.</span><span class="sxs-lookup"><span data-stu-id="5cc23-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="5cc23-113">[Používanie atribútov prípony v adresárových schémach v žiadostiach](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) popisuje, ako používať atribúty prípony adresárovej schémy na odosielanie používateľských údajov do aplikácií v tokenových pohľadávkach.</span><span class="sxs-lookup"><span data-stu-id="5cc23-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="5cc23-114">Ďalšie informácie o tokenových pohľadávkach nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="5cc23-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="5cc23-115">Pohľadávky v accessových tokenoch</span><span class="sxs-lookup"><span data-stu-id="5cc23-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="5cc23-116">Nároky v id_token</span><span class="sxs-lookup"><span data-stu-id="5cc23-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="5cc23-117">[Požiadavky](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , ktoré možno očakávať v tokenoch identifikácie a prístupových tokenoch vydaných službou Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="5cc23-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="5cc23-118">Odkaz na deklaráciu SAML tokenu</span><span class="sxs-lookup"><span data-stu-id="5cc23-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
