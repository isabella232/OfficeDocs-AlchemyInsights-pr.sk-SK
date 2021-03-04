---
title: Riešenie problémov s SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430215"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="20186-102">Riešenie problémov s SSPR</span><span class="sxs-lookup"><span data-stu-id="20186-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="20186-103">**Mám problémy s konfiguráciou nového hesla**</span><span class="sxs-lookup"><span data-stu-id="20186-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="20186-104">Ak ste správcom a hľadáte spôsob, ako povoliť samoobslužné vytvorenie nového hesla, pozrite si tému [povolenie SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)na konfigurovanie obnovenia nového hesla pre vašu organizáciu.</span><span class="sxs-lookup"><span data-stu-id="20186-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="20186-105">Môžete tiež skontrolovať [licenčné požiadavky](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="20186-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="20186-106">V organizácii musíte mať priradenú aspoň jednu licenciu.</span><span class="sxs-lookup"><span data-stu-id="20186-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="20186-107">**Iba používatelia cloudu** – všetky platené jednotky SKU služieb Office 365 (O365) alebo Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="20186-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="20186-108">**Cloudové a/alebo lokálne používatelia** – Azure AD Premium P1 alebo P2, Enterprise mobility + Security (EMS) alebo zabezpečený produktívny podnik (SPE)</span><span class="sxs-lookup"><span data-stu-id="20186-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="20186-109">Ďalšie otázky o automatickom resetovaní hesla nájdete v [téme Najčastejšie otázky](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="20186-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="20186-110">**Zobrazuje sa chybové hlásenie**</span><span class="sxs-lookup"><span data-stu-id="20186-110">**I'm getting an error message**</span></span>

<span data-ttu-id="20186-111">V tomto článku nájdete informácie o bežných chybách a ich riešeniach: [Riešenie problémov s vlastným servisným vynulovaním hesla](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="20186-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="20186-112">**Mám problém s politikou na vytvorenie nového hesla**</span><span class="sxs-lookup"><span data-stu-id="20186-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="20186-113">Ak sa politika obnovenia hesla nespráva podľa očakávaní alebo ak máte otázky týkajúce sa politík na vytvorenie nového hesla, prečítajte si tento článok: [politiky a obmedzenia hesiel v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="20186-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="20186-114">Politiky na vytvorenie nového hesla sa nevzťahujú na správcov.</span><span class="sxs-lookup"><span data-stu-id="20186-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="20186-115">Spoločnosť Microsoft vynúti silnú predvolenú politiku na vytvorenie nového hesla s dvoma bránami pre ľubovoľnú rolu správcu služby Azure.</span><span class="sxs-lookup"><span data-stu-id="20186-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="20186-116">Uistite sa, že skúšate používateľa, ktorý nie je správcom.</span><span class="sxs-lookup"><span data-stu-id="20186-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="20186-117">Ďalšie informácie o politike obnovenia správcu nájdete v téme tento článok: [Obnovenie zásad politiky správcu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="20186-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="20186-118">**Nechcem, aby moji používatelia zaregistrovali ďalšie bezpečnostné informácie na vytvorenie nového hesla**</span><span class="sxs-lookup"><span data-stu-id="20186-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="20186-119">Pre používateľov môžete vopred vyplniť údaje (e-maily a telefónne atribúty) pomocou rozhrania API, PowerShell alebo služby Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="20186-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="20186-120">Ak sa chcete dozvedieť, ako čítať:</span><span class="sxs-lookup"><span data-stu-id="20186-120">To learn how read:</span></span>

- [<span data-ttu-id="20186-121">Nasadenie nového hesla bez nutnosti registrácie používateľov</span><span class="sxs-lookup"><span data-stu-id="20186-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="20186-122">Aké údaje sa používajú na vytvorenie nového hesla</span><span class="sxs-lookup"><span data-stu-id="20186-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="20186-123">**Chcem, aby moji používatelia zaregistrovali ďalšie bezpečnostné informácie na vytvorenie nového hesla**</span><span class="sxs-lookup"><span data-stu-id="20186-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="20186-124">Požiadajte svojich používateľov, aby si zaregistrovali svoje bezpečnostné informácie na vytvorenie nového hesla a nasmerujú ich na [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).</span><span class="sxs-lookup"><span data-stu-id="20186-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="20186-125">Po vyplnení údajov používateľovi (používateľom alebo správcom) nasmerujte používateľa na [aka.MS/SSPR](https://passwordreset.microsoftonline.com/) , aby mohli vaši používatelia mať právo na vytvorenie nového hesla.</span><span class="sxs-lookup"><span data-stu-id="20186-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="20186-126">Ak sa stále vyskytujú problémy, ktoré sú s najväčšou pravdepodobnosťou **externý** alebo **hash hesla synchronizovaní** používatelia.</span><span class="sxs-lookup"><span data-stu-id="20186-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="20186-127">To znamená, že je pravdepodobné, že sa vyskytol problém so službou Password zápisom.</span><span class="sxs-lookup"><span data-stu-id="20186-127">This means there is likely a problem with the Password Writeback service.</span></span>