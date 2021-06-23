---
title: Zapnutie overovania SMTP a riešenie problémov
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077666"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="d3603-102">Zapnutie overovania SMTP a riešenie problémov</span><span class="sxs-lookup"><span data-stu-id="d3603-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="d3603-103">Ak chcete zapnúť overenie SMTP pre poštovú schránku alebo sa vám zobrazuje chyba Klient nie je overený, Overenie neúspešné alebo SmtpClientAuthentication s kódom 5.7.57 alebo 5.7.3 alebo 5.7.139 pri pokuse o prenos e-mailov overením zariadenia alebo aplikácie so systémom Microsoft 365, problém vyriešte vykonaním týchto troch akcií:</span><span class="sxs-lookup"><span data-stu-id="d3603-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="d3603-104">Ak chcete [vypnúť predvolené nastavenia zabezpečenia služby Azure,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) prepnite možnosť Povoliť predvolené nastavenia zabezpečenia **na** **možnosť Nie.**</span><span class="sxs-lookup"><span data-stu-id="d3603-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="d3603-105">a.</span><span class="sxs-lookup"><span data-stu-id="d3603-105">a.</span></span> <span data-ttu-id="d3603-106">Prihláste sa na portál Azure ako správca zabezpečenia, správca podmieneného prístupu alebo globálny správca.</span><span class="sxs-lookup"><span data-stu-id="d3603-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="d3603-107">b.</span><span class="sxs-lookup"><span data-stu-id="d3603-107">b.</span></span> <span data-ttu-id="d3603-108">Prejdite na Azure Active Directory > **Vlastnosti.**</span><span class="sxs-lookup"><span data-stu-id="d3603-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="d3603-109">c.</span><span class="sxs-lookup"><span data-stu-id="d3603-109">c.</span></span> <span data-ttu-id="d3603-110">Vyberte **položku Správa predvolených nastavení zabezpečenia.**</span><span class="sxs-lookup"><span data-stu-id="d3603-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="d3603-111">d.</span><span class="sxs-lookup"><span data-stu-id="d3603-111">d.</span></span> <span data-ttu-id="d3603-112">Nastavte **položku Povoliť predvolené nastavenia zabezpečenia** na možnosť **Nie.**</span><span class="sxs-lookup"><span data-stu-id="d3603-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="d3603-113">e.</span><span class="sxs-lookup"><span data-stu-id="d3603-113">e.</span></span> <span data-ttu-id="d3603-114">Vyberte **položku Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="d3603-114">Select **Save**.</span></span>

2. <span data-ttu-id="d3603-115">[Povoľte odosielanie klientskeho SMTP](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) servera v licencovanej poštovej schránke.</span><span class="sxs-lookup"><span data-stu-id="d3603-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="d3603-116">a.</span><span class="sxs-lookup"><span data-stu-id="d3603-116">a.</span></span> <span data-ttu-id="d3603-117">V Centrum spravovania služby Microsoft 365 prejdite na **položku Aktívni** používatelia a vyberte používateľa.</span><span class="sxs-lookup"><span data-stu-id="d3603-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="d3603-118">b.</span><span class="sxs-lookup"><span data-stu-id="d3603-118">b.</span></span> <span data-ttu-id="d3603-119">Prejdite na kartu Pošta a v časti **E-mailové aplikácie vyberte** položku Spravovať **e-mailové aplikácie**.</span><span class="sxs-lookup"><span data-stu-id="d3603-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="d3603-120">d.</span><span class="sxs-lookup"><span data-stu-id="d3603-120">d.</span></span> <span data-ttu-id="d3603-121">Skontrolujte, **či je začiarknuté políčko** Overený SMTP server (zapnuté).</span><span class="sxs-lookup"><span data-stu-id="d3603-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="d3603-122">e.</span><span class="sxs-lookup"><span data-stu-id="d3603-122">e.</span></span> <span data-ttu-id="d3603-123">Vyberte **položku Save changes (Uložiť zmeny).**</span><span class="sxs-lookup"><span data-stu-id="d3603-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="d3603-124">[V licencovanej poštovej schránke vypnite](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) viacfaktorové overovanie.</span><span class="sxs-lookup"><span data-stu-id="d3603-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="d3603-125">a.</span><span class="sxs-lookup"><span data-stu-id="d3603-125">a.</span></span> <span data-ttu-id="d3603-126">Prejdite na navigačnú Centrum spravovania služby Microsoft 365 a v ľavej navigačnej ponuke vyberte položku **Používatelia**  >  **Aktívni používatelia.**</span><span class="sxs-lookup"><span data-stu-id="d3603-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="d3603-127">b.</span><span class="sxs-lookup"><span data-stu-id="d3603-127">b.</span></span> <span data-ttu-id="d3603-128">Vyberte **položku Viacfaktorové overovanie.**</span><span class="sxs-lookup"><span data-stu-id="d3603-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="d3603-129">c.</span><span class="sxs-lookup"><span data-stu-id="d3603-129">c.</span></span> <span data-ttu-id="d3603-130">Vyberte používateľa a vypnite **možnosť Viacfaktorové overovanie.**</span><span class="sxs-lookup"><span data-stu-id="d3603-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
