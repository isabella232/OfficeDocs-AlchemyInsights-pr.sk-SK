---
title: Rola s privilegovaným správaním identity
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089152"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="52954-102">Rola správy privilegovaných identít (PIM)</span><span class="sxs-lookup"><span data-stu-id="52954-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="52954-103">**Povolenia sa neudelia po aktivácii roly**</span><span class="sxs-lookup"><span data-stu-id="52954-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="52954-104">Pri aktivácii roly v službe Azure AD privileged Identity Management (PIM) sa aktivácia nemusí okamžite rozšíriť na všetky portály, ktoré vyžadujú privilegovanú rolu.</span><span class="sxs-lookup"><span data-stu-id="52954-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="52954-105">Niekedy aj v prípade, že sa zmena rozšírila, web caching na portáli môže mať za následok zmeny, ktoré sa neprejavia okamžite.</span><span class="sxs-lookup"><span data-stu-id="52954-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="52954-106">Ak je vaša Aktivácia oneskorená, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="52954-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="52954-107">Odhláste sa zo služby Azure Portal a potom sa znova prihláste.</span><span class="sxs-lookup"><span data-stu-id="52954-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="52954-108">Keď aktivujete rolu Azure AD alebo rolu Azure Resource, zobrazia sa vám fázy aktivácie.</span><span class="sxs-lookup"><span data-stu-id="52954-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="52954-109">Po dokončení všetkých fáz sa zobrazí prepojenie odhlásiť sa.</span><span class="sxs-lookup"><span data-stu-id="52954-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="52954-110">Ak sa chcete odhlásiť, môžete použiť toto prepojenie. Tým sa vyrieši väčšina prípadov oneskorenia aktivácie.</span><span class="sxs-lookup"><span data-stu-id="52954-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="52954-111">V PIM Skontrolujte, či ste ako člen roly zaradení.</span><span class="sxs-lookup"><span data-stu-id="52954-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="52954-112">Ak aktivujete rolu správcu servera Exchange, skontrolujte, či sa odhlásite a znova prihlásite.</span><span class="sxs-lookup"><span data-stu-id="52954-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="52954-113">Ak problém pretrváva, otvorte lístok technickej podpory a Vyzdvihnite ho ako problém.</span><span class="sxs-lookup"><span data-stu-id="52954-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="52954-114">Ak používate rolu správcu servera Exchange na prístup k centru zabezpečenia a dodržiavania súladu, pozrite si ďalší krok.</span><span class="sxs-lookup"><span data-stu-id="52954-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="52954-115">Ak aktivujete rolu na prístup k centru zabezpečenia a dodržiavania súladu, alebo Ak aktivujete rolu správcu služby SharePoint, niektoré oneskorené aktivácie sa vyskytnú od niekoľkých minút až do niekoľkých hodín.</span><span class="sxs-lookup"><span data-stu-id="52954-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="52954-116">Toto je známy problém a aktívne pracujeme s týmito tímami na vyriešenie tohto problému čo najskôr.</span><span class="sxs-lookup"><span data-stu-id="52954-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="52954-117">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="52954-117">For more information, see:</span></span>

- [<span data-ttu-id="52954-118">Aktivácia rol služby Azure AD v PIM</span><span class="sxs-lookup"><span data-stu-id="52954-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="52954-119">Aktivácia rolí Azure Resource v PIM</span><span class="sxs-lookup"><span data-stu-id="52954-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="52954-120">**Povolenia sa neodstránia po deaktivácii roly alebo po uplynutí platnosti aktivácie roly**</span><span class="sxs-lookup"><span data-stu-id="52954-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="52954-121">Keď deaktivujete rolu v službe Azure AD privilegovaná správa identít alebo po uplynutí obdobia aktivácie roly, môže sa stať, že budete mať naďalej prístup.</span><span class="sxs-lookup"><span data-stu-id="52954-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="52954-122">Ak sa deaktivácia oneskorí, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="52954-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="52954-123">Ak deaktivujete rolu správcu servera Exchange alebo uplynie obdobie aktivácie roly a zistíte, že pred odstránením povolení uplynulo značné oneskorenie, otvorte lístok technickej podpory a informujte svojho pracovníka technickej podpory, aby vám pomohol pomenovať letenku s tímom PAM (privilegovaný prístup Management) v rámci balíka Office o tomto probléme.</span><span class="sxs-lookup"><span data-stu-id="52954-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="52954-124">Ak uplynula platnosť obdobia aktivácie, ale stále máte otvorenú reláciu prehliadača, ukončite prehliadač.</span><span class="sxs-lookup"><span data-stu-id="52954-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="52954-125">Rolu môžete naďalej používať, až kým nezavriete danú reláciu.</span><span class="sxs-lookup"><span data-stu-id="52954-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="52954-126">Ide o známy problém a my sa pozrieme na možnú opravu, aby ste po uplynutí platnosti aktivácie aktívne zrušili každú reláciu.</span><span class="sxs-lookup"><span data-stu-id="52954-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="52954-127">Ak je oneskorenie iné ako tieto dva scenáre, otvorte lístok technickej podpory.</span><span class="sxs-lookup"><span data-stu-id="52954-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
