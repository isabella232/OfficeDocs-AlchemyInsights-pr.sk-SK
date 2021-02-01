---
title: Problémy s povereniami
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063687"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="f1322-102">Problémy s povereniami</span><span class="sxs-lookup"><span data-stu-id="f1322-102">Issues with credentials</span></span>

<span data-ttu-id="f1322-103">[Platforma Microsoft identity a tok poverení klienta oauth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) popisujú, ako program priamo v porovnaní s povereniami klienta OAuth 2,0 udeliť tok.</span><span class="sxs-lookup"><span data-stu-id="f1322-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="f1322-104">**Ako môžem spravovať poverenia na zadanie hesla alebo certifikátu aplikácie?**</span><span class="sxs-lookup"><span data-stu-id="f1322-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="f1322-105">V platforme Azure CLI môžete na odstránenie, zoznam alebo vynulovanie poverení hesla alebo certifikátu aplikácie použiť [poverenia služby AZ ad](https://docs.microsoft.com/cli/azure/ad/app/credential) .</span><span class="sxs-lookup"><span data-stu-id="f1322-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="f1322-106">**Ako si používatelia vynulujú svoje heslá?**</span><span class="sxs-lookup"><span data-stu-id="f1322-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="f1322-107">Používatelia sa musia [zaregistrovať na samoobslužné vytvorenie nového hesla](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) predtým, ako budú môcť obnoviť svoje heslá.</span><span class="sxs-lookup"><span data-stu-id="f1322-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="f1322-108">Keď sa používateľ zaregistroval, môže podľa pokynov v tomto článku vytvoriť nové heslo: [Vytvorenie nového pracovného alebo školského hesla](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="f1322-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="f1322-109">**Ako používatelia zmenia svoje heslá?**</span><span class="sxs-lookup"><span data-stu-id="f1322-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="f1322-110">Používatelia môžu postupovať podľa krokov v tomto článku na zmenu hesla: [ako zmeniť heslo](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="f1322-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="f1322-111">Môžu tiež [Spravovať heslá aplikácií pre dvojstupňové overovanie](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="f1322-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="f1322-112">**Používateľovi sa zobrazuje chyba pri zmene alebo resetovaní hesla**</span><span class="sxs-lookup"><span data-stu-id="f1322-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="f1322-113">Toto prepojenie poskytne informácie o bežných problémoch, ktoré sa môžu vyskytnúť pri pokuse používateľa o vytvorenie nového hesla: [bežné problémy a ich riešenia](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="f1322-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="f1322-114">**Mám problém s obnovením hesla používateľa**</span><span class="sxs-lookup"><span data-stu-id="f1322-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="f1322-115">Uistite sa, že máte oprávnenie na vytvorenie nového hesla.</span><span class="sxs-lookup"><span data-stu-id="f1322-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="f1322-116">*Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov.*</span><span class="sxs-lookup"><span data-stu-id="f1322-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="f1322-117">Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.</span><span class="sxs-lookup"><span data-stu-id="f1322-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="f1322-118">Uistite sa, že chápete licenčné požiadavky:</span><span class="sxs-lookup"><span data-stu-id="f1322-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="f1322-119">V organizácii musíte mať priradenú aspoň jednu licenciu:</span><span class="sxs-lookup"><span data-stu-id="f1322-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="f1322-120">**Iba používatelia cloudu** – všetky platené jednotky SKU služieb Office 365 (O365) alebo Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="f1322-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="f1322-121">**Cloudové a/alebo lokálne používatelia** – Azure AD Premium P1 alebo P2, Enterprise mobility + Security (EMS) alebo zabezpečený produktívny podnik (SPE)</span><span class="sxs-lookup"><span data-stu-id="f1322-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="f1322-122">Ďalšie informácie o licenčných požiadavkách nájdete [v téme licenčné požiadavky na vytvorenie nového hesla služby Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="f1322-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="f1322-123">Ak chcete vytvoriť nové heslo používateľa, vyhľadajte používateľa v službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1322-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="f1322-124">Potom v prehľade Blade pre daného používateľa kliknite na tlačidlo vytvoriť nové heslo.</span><span class="sxs-lookup"><span data-stu-id="f1322-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="f1322-125">**Tlačidlo na vytvorenie nového hesla je sivé**</span><span class="sxs-lookup"><span data-stu-id="f1322-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="f1322-126">Nemáte oprávnenie na vytvorenie nového hesla **tohto** používateľa.</span><span class="sxs-lookup"><span data-stu-id="f1322-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="f1322-127">*Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov.*</span><span class="sxs-lookup"><span data-stu-id="f1322-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="f1322-128">Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.</span><span class="sxs-lookup"><span data-stu-id="f1322-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="f1322-129">**Nezobrazuje sa vám čepeľ na vytvorenie nového hesla**</span><span class="sxs-lookup"><span data-stu-id="f1322-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="f1322-130">Nemáte oprávnenie na vytvorenie nového hesla.</span><span class="sxs-lookup"><span data-stu-id="f1322-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="f1322-131">*Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov.*</span><span class="sxs-lookup"><span data-stu-id="f1322-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="f1322-132">Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.</span><span class="sxs-lookup"><span data-stu-id="f1322-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="f1322-133">**V časti Vytvorenie nového hesla sa nezobrazuje lokálna integračná čepeľ**</span><span class="sxs-lookup"><span data-stu-id="f1322-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="f1322-134">Lokálna integračná čepeľ sa zobrazuje len v hybridných prostrediach, čo znamená, že používate heslo zápisom na manipuláciu s heslami lokálneho používateľa.</span><span class="sxs-lookup"><span data-stu-id="f1322-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="f1322-135">Táto čepeľ sa nezobrazuje, ak:</span><span class="sxs-lookup"><span data-stu-id="f1322-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="f1322-136">Nepoužívate heslo zápisom</span><span class="sxs-lookup"><span data-stu-id="f1322-136">You are not using password writeback</span></span>
  - <span data-ttu-id="f1322-137">Vyskytol sa problém s inštaláciou alebo pripojením hesla zápisom</span><span class="sxs-lookup"><span data-stu-id="f1322-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="f1322-138">Vyskytol sa problém s inštaláciou alebo pripojením služby Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f1322-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="f1322-139">Ďalšie kroky na riešenie problémov s heslom zápisom nájdete v téme [Riešenie problémov s heslom zápisom](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="f1322-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="f1322-140">**Neviem, ako vytvoriť nové heslo používateľa**</span><span class="sxs-lookup"><span data-stu-id="f1322-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="f1322-141">Prihláste sa na portáli Azure ako príslušný správca.</span><span class="sxs-lookup"><span data-stu-id="f1322-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="f1322-142">Prejdite na čepeľ **Používatelia a skupiny** , vyberte položku **všetci používatelia**.</span><span class="sxs-lookup"><span data-stu-id="f1322-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="f1322-143">Vyberte používateľa v zozname.</span><span class="sxs-lookup"><span data-stu-id="f1322-143">Select a user from the list.</span></span>
4. <span data-ttu-id="f1322-144">Pre vybratého používateľa vyberte položku **Prehľad** a potom na paneli príkazov vyberte položku **vytvoriť nové heslo**.</span><span class="sxs-lookup"><span data-stu-id="f1322-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="f1322-145">Vyberte tlačidlo **vynulovať heslo** a postupujte podľa pokynov na obrazovke.</span><span class="sxs-lookup"><span data-stu-id="f1322-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="f1322-146">Obnoví sa len prostredníctvom zápisom hesla podpory **platformy Azure Portal** .</span><span class="sxs-lookup"><span data-stu-id="f1322-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="f1322-147">**Pri resetovaní hesla lokálneho používateľa na portáli pre správcov služieb Office 365 alebo v mobilnej aplikácii balíka Office 365 sa používateľ stále nedokáže prihlásiť**</span><span class="sxs-lookup"><span data-stu-id="f1322-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="f1322-148">Na tomto portáli nie je podporovaná zápisom hesla.</span><span class="sxs-lookup"><span data-stu-id="f1322-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="f1322-149">Znova obnovte heslo používateľa na portáli Azure.</span><span class="sxs-lookup"><span data-stu-id="f1322-149">Reset the user's password again in the Azure portal.</span></span>
