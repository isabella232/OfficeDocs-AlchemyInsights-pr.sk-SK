---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820193"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="6eca4-102">Blokovanie staršieho overovania</span><span class="sxs-lookup"><span data-stu-id="6eca4-102">Blocking legacy authentication</span></span>

<span data-ttu-id="6eca4-103">Staršie overovanie je výraz, ktorý odkazuje na žiadosť o overenie, ktorú:</span><span class="sxs-lookup"><span data-stu-id="6eca4-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="6eca4-104">Starší klienti Office, ktorí používajú moderné overovanie (napríklad klient Office 2010).</span><span class="sxs-lookup"><span data-stu-id="6eca4-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="6eca4-105">akéhokoľvek klienta, ktorý používa staršie poštové protokoly, ako napríklad IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="6eca4-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="6eca4-106">Ďalšie informácie o blokovaní staršieho overovania a povolení moderného overovania nájdete v časti [Blokovanie staršieho overovania.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="6eca4-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="6eca4-107">Predvolené nastavenia zabezpečenia v Azure Active Directory (Azure AD) uľahčujú zabezpečenie a pomáhajú chrániť vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="6eca4-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="6eca4-108">Predvolené nastavenia zabezpečenia obsahujú vopred nakonfigurované nastavenia zabezpečenia pre bežné útoky.</span><span class="sxs-lookup"><span data-stu-id="6eca4-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="6eca4-109">Ďalšie informácie o predvolených nastaveniach zabezpečenia nájdete v [časti Čo sú predvolené nastavenia zabezpečenia?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="6eca4-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="6eca4-110">**Poznámka:** Ak bol váš nájomník vytvorený 22. októbra 2019 alebo po ňom, je možné, že sa v ňom vyskytujú nové predvolene zabezpečené správanie a v nájomníkovi už sú zapnuté predvolené nastavenia zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="6eca4-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="6eca4-111">V snahe chrániť všetkých našich používateľov sa pre všetkých nových vytvorených nájomníkov s cieľom chrániť predvolené hodnoty zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="6eca4-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
