---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685613"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="dec71-102">Blokovanie starších overovaní</span><span class="sxs-lookup"><span data-stu-id="dec71-102">Blocking legacy authentication</span></span>

<span data-ttu-id="dec71-103">Staršie overovanie je výraz, ktorý odkazuje na žiadosť o overenie vykonanú:</span><span class="sxs-lookup"><span data-stu-id="dec71-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="dec71-104">Starší klienti balíka Office, ktorí nepoužívajú moderné overovanie (napríklad klient služieb Office 2010).</span><span class="sxs-lookup"><span data-stu-id="dec71-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="dec71-105">Každý klient, ktorý používa staršie poštové protokoly, ako napríklad IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="dec71-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="dec71-106">Ďalšie informácie o blokovaní starších overovaní a povolení moderného overovania nájdete v téme [blokovanie starších overovaní](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="dec71-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="dec71-107">Predvolené nastavenie zabezpečenia v službe Azure Active Directory (Azure AD) uľahčuje zabezpečenie a pomáha chrániť vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="dec71-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="dec71-108">Predvolené nastavenie zabezpečenia obsahuje vopred nakonfigurované nastavenia zabezpečenia bežných útokov.</span><span class="sxs-lookup"><span data-stu-id="dec71-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="dec71-109">Ďalšie informácie o predvolených nastaveniach zabezpečenia nájdete v téme [čo sú predvolené nastavenia zabezpečenia?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="dec71-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="dec71-110">**Poznámka**: Ak bol váš nájomník vytvorený alebo po 22. října, 2019, je možné, že sa vyskytli nové správanie na základe zabezpečeného predvoleného nastavenia a už máte v nájomníkovi povolené predvolené nastavenia zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="dec71-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="dec71-111">V snahe ochrániť všetkých našich používateľov sú predvolené hodnoty zabezpečenia vyradené všetkým novým nájomníkom vytvoreným.</span><span class="sxs-lookup"><span data-stu-id="dec71-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
