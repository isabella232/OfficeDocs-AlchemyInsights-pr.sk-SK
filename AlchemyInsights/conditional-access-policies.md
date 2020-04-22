---
title: Politiky podmieneného prístupu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 569507318b499cdbcf2a1cd75e84046953f62212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706072"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="54abc-102">Politiky podmieneného prístupu</span><span class="sxs-lookup"><span data-stu-id="54abc-102">Conditional Access policies</span></span>

<span data-ttu-id="54abc-103">Podmienený prístup je funkcia služby Azure AD, ktorá umožňuje vynútiť ovládacie prvky prístupu k aplikáciám vo vašom prostredí a to všetko na základe konkrétnych podmienok so spravovaním z centrálneho umiestnenia.</span><span class="sxs-lookup"><span data-stu-id="54abc-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="54abc-104">Ďalšie informácie o [podmienenom prístupe služby Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="54abc-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="54abc-105">**Poznámka**: Ak bol váš nájomník vytvorený po 21. októbri 2019 a neočakávane sa vám zobrazí výzva na viacfaktorové overenie, pravdepodobne máte pre svojho nájomníka aktivované [predvolené nastavenia zabezpečenia](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="54abc-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="54abc-106">**Ak chcete spravovať predvolené nastavenia zabezpečenia**</span><span class="sxs-lookup"><span data-stu-id="54abc-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="54abc-107">Prihláste sa do [Centra spravovania](https://go.microsoft.com/fwlink/p/?linkid=834822) pomocou poverení globálneho správcu.</span><span class="sxs-lookup"><span data-stu-id="54abc-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="54abc-108">Prejdite do časti [Vlastnosti Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)</span><span class="sxs-lookup"><span data-stu-id="54abc-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="54abc-109">V dolnej časti stránky kliknite na položku **Spravovanie predvolených nastavení zabezpečenia**.</span><span class="sxs-lookup"><span data-stu-id="54abc-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="54abc-110">Kliknutím na položku **Áno** povolíte predvolené nastavenia zabezpečenia alebo kliknutím na položku **Nie** vypnete predvolené nastavenia zabezpečenia.</span><span class="sxs-lookup"><span data-stu-id="54abc-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
