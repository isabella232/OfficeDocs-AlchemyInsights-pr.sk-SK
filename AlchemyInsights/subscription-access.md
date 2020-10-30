---
title: Prístup k predplatnému
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807721"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="8ee6c-102">Azure sa nedá prihlásiť v dôsledku problémov s prehliadačom (prehliadač sa zablokuje, udržuje spinning, nenačíta sa atď.)</span><span class="sxs-lookup"><span data-stu-id="8ee6c-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="8ee6c-103">Môže sa stať, že budete mať vplyv na výpadok.</span><span class="sxs-lookup"><span data-stu-id="8ee6c-103">You might be impacted by an outage.</span></span> <span data-ttu-id="8ee6c-104">Skontrolujte, či sa vyskytol pokračujúci výpadok: [stav služby Azure Health](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="8ee6c-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="8ee6c-105">Odhláste sa zo všetkých aktívnych relácií služby Azure.</span><span class="sxs-lookup"><span data-stu-id="8ee6c-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="8ee6c-106">Spustite režim v súkromí alebo v režime inkognito webového prehliadača.</span><span class="sxs-lookup"><span data-stu-id="8ee6c-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="8ee6c-107">Môžete sa tiež pokúsiť obnoviť prehliadač, použiť iný prehliadač, odstrániť súbory cookie vyrovnávacej pamäte, ak vyššie uvedené nefunguje.</span><span class="sxs-lookup"><span data-stu-id="8ee6c-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="8ee6c-108">Ďalšie informácie: [Riešenie problémov s prihlasovaním](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="8ee6c-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="8ee6c-109">**Nie je možné získať prístup k predplatnému**</span><span class="sxs-lookup"><span data-stu-id="8ee6c-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="8ee6c-110">Na [portáli Azure](https://portal.azure.com/)Skontrolujte, či je v pravom hornom rohu vybratá správna adresár Azure.</span><span class="sxs-lookup"><span data-stu-id="8ee6c-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="8ee6c-111">Skontrolujte, či je v [centre Azure Account](https://account.windowsazure.com/Subscriptions)(konto) konto správcu konta.</span><span class="sxs-lookup"><span data-stu-id="8ee6c-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="8ee6c-112">Ďalšie informácie: [Riešenie problémov s nenájdenými predplatnými](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="8ee6c-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="8ee6c-113">**Nie je možné získať prístup k histórii fakturácie**</span><span class="sxs-lookup"><span data-stu-id="8ee6c-113">**Unable to access billing history**</span></span>

<span data-ttu-id="8ee6c-114">Správca konta potrebuje uistiť sa, že používateľ s prístupom k informáciám o fakturácii sa pridá do služby Azure Active Directory ako hosťovský používateľ: [Pridanie alebo odstránenie nového používateľa](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8ee6c-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="8ee6c-115">Používateľovi sa potom musí dostať rola globálneho správcu: [Priradenie roly používateľom](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8ee6c-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="8ee6c-116">Zverejniť tento príspevok môže mať používateľ prístup na fakturáciu pomocou politík RBAC: [udelenie prístupu k fakturácii](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8ee6c-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="8ee6c-117">**Odporúčané dokumenty**</span><span class="sxs-lookup"><span data-stu-id="8ee6c-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="8ee6c-118">Nemôžem sa prihlásiť na spravovanie môjho predplatného Azure</span><span class="sxs-lookup"><span data-stu-id="8ee6c-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)