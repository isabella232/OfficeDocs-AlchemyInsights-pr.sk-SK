---
title: Problém s obnovením hesla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696277"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="aaf17-102">Problémy s obnovením hesla</span><span class="sxs-lookup"><span data-stu-id="aaf17-102">Problems resetting password</span></span>

<span data-ttu-id="aaf17-103">Nižšie sú uvedené niektoré problémy, s ktorými sa môžete stretnúť pri resetovaní hesla a možných riešeniach:</span><span class="sxs-lookup"><span data-stu-id="aaf17-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="aaf17-104">**Mám problém s vytvorením nového hesla, ktoré nie je zahrnuté v iných kategóriách**</span><span class="sxs-lookup"><span data-stu-id="aaf17-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="aaf17-105">Uistite sa, že máte oprávnenie na vytvorenie nového hesla.</span><span class="sxs-lookup"><span data-stu-id="aaf17-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="aaf17-106">Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov.</span><span class="sxs-lookup"><span data-stu-id="aaf17-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="aaf17-107">Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.</span><span class="sxs-lookup"><span data-stu-id="aaf17-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="aaf17-108">Uistite sa, že chápete licenčné požiadavky:</span><span class="sxs-lookup"><span data-stu-id="aaf17-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="aaf17-109">V organizácii musíte mať priradenú aspoň jednu licenciu.</span><span class="sxs-lookup"><span data-stu-id="aaf17-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="aaf17-110">Iba používatelia cloudu – všetky platené jednotky SKU služieb Office 365 (O365) alebo Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="aaf17-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="aaf17-111">Cloudové a/alebo lokálne používatelia – Azure AD Premium P1 alebo P2, Enterprise mobility + Security (EMS) alebo zabezpečený produktívny podnik (SPE)</span><span class="sxs-lookup"><span data-stu-id="aaf17-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="aaf17-112">Ďalšie informácie o licenčných požiadavkách nájdete v článku [licenčné požiadavky na vytvorenie nového hesla služby Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="aaf17-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="aaf17-113">**Mám problémy s testovaním politiky na vytvorenie nového hesla**</span><span class="sxs-lookup"><span data-stu-id="aaf17-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="aaf17-114">Naposledy aplikované politiky môžu trvať niekoľko minút, kým sa replikujú vo všetkých dátových centrách a na koncových bodoch.</span><span class="sxs-lookup"><span data-stu-id="aaf17-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="aaf17-115">Fyzická vzdialenosť od dátového centra ovplyvní aj spôsob používania rýchlych zmien.</span><span class="sxs-lookup"><span data-stu-id="aaf17-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="aaf17-116">Otestujte sa koncovým používateľom, nie správcom, a pilot s malou skupinou používateľov.</span><span class="sxs-lookup"><span data-stu-id="aaf17-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="aaf17-117">Politiky nakonfigurované na portáli Azure sa uplatňujú len na koncových používateľov, nie správcov.</span><span class="sxs-lookup"><span data-stu-id="aaf17-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="aaf17-118">Spoločnosť Microsoft vynúti silnú predvolenú politiku na vytvorenie nového hesla s dvoma bránami pre ľubovoľnú rolu správcu služby Azure (príklad: globálny správca, správca helpdesk, správca hesiel atď.)</span><span class="sxs-lookup"><span data-stu-id="aaf17-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="aaf17-119">Ďalšie informácie o [politikách pre správcov](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="aaf17-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="aaf17-120">**Chcem nasadiť vytvorenie nového hesla, ale nechcem, aby moji používatelia zaregistrovali ďalšie bezpečnostné informácie**</span><span class="sxs-lookup"><span data-stu-id="aaf17-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="aaf17-121">Pred vyplnením údajov pre používateľov tak, aby nemuseli.</span><span class="sxs-lookup"><span data-stu-id="aaf17-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="aaf17-122">-Ako správca môžete nastaviť vlastnosti telefónu a e-mailu pre svojich používateľov pred vykonaním obnovenia nového hesla vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="aaf17-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="aaf17-123">Môžete to urobiť pomocou rozhrania API, PowerShell alebo Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="aaf17-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="aaf17-124">Ďalšie informácie nájdete tu:</span><span class="sxs-lookup"><span data-stu-id="aaf17-124">More information here:</span></span>
- [<span data-ttu-id="aaf17-125">Nasadenie nového hesla bez nutnosti registrácie používateľov</span><span class="sxs-lookup"><span data-stu-id="aaf17-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="aaf17-126">Aké údaje sa používajú na vytvorenie nového hesla</span><span class="sxs-lookup"><span data-stu-id="aaf17-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="aaf17-127">**Tlačidlo na vytvorenie nového hesla je sivé**</span><span class="sxs-lookup"><span data-stu-id="aaf17-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="aaf17-128">Nemáte oprávnenie na vytvorenie nového hesla tohto používateľa.</span><span class="sxs-lookup"><span data-stu-id="aaf17-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="aaf17-129">Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov.</span><span class="sxs-lookup"><span data-stu-id="aaf17-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="aaf17-130">Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.</span><span class="sxs-lookup"><span data-stu-id="aaf17-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="aaf17-131">**Nezobrazuje sa vám čepeľ na vytvorenie nového hesla**</span><span class="sxs-lookup"><span data-stu-id="aaf17-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="aaf17-132">Nemáte oprávnenie na vytvorenie nového hesla.</span><span class="sxs-lookup"><span data-stu-id="aaf17-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="aaf17-133">Heslá používateľov môžu vynulovať len globálne, heslo a správcovia používateľov.</span><span class="sxs-lookup"><span data-stu-id="aaf17-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="aaf17-134">Globálni správcovia môžu tiež obnoviť heslá ostatných privilegovaných správcov.</span><span class="sxs-lookup"><span data-stu-id="aaf17-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="aaf17-135">**V časti Vytvorenie nového hesla sa nezobrazuje lokálna integračná čepeľ**</span><span class="sxs-lookup"><span data-stu-id="aaf17-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="aaf17-136">Lokálna integračná čepeľ sa zobrazuje len v hybridných prostrediach, čo znamená, že používate heslo zápisom na manipuláciu s heslami lokálneho používateľa.</span><span class="sxs-lookup"><span data-stu-id="aaf17-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="aaf17-137">Táto čepeľ sa nezobrazuje, ak:</span><span class="sxs-lookup"><span data-stu-id="aaf17-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="aaf17-138">Nepoužívate heslo zápisom</span><span class="sxs-lookup"><span data-stu-id="aaf17-138">You are not using password writeback</span></span>
    - <span data-ttu-id="aaf17-139">Vyskytol sa problém s inštaláciou alebo pripojením hesla zápisom</span><span class="sxs-lookup"><span data-stu-id="aaf17-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="aaf17-140">Vyskytol sa problém s inštaláciou alebo pripojením služby Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="aaf17-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="aaf17-141">Ďalšie kroky na riešenie problémov s heslom zápisom nájdete v časti [Riešenie problémov s heslom zápisom](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="aaf17-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="aaf17-142">**Neviem, ako vytvoriť nové heslo používateľa**</span><span class="sxs-lookup"><span data-stu-id="aaf17-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="aaf17-143">Prihláste sa na portáli Azure ako príslušný správca.</span><span class="sxs-lookup"><span data-stu-id="aaf17-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="aaf17-144">Prejdite na čepeľ používatelia a skupiny, vyberte položku **všetci používatelia**.</span><span class="sxs-lookup"><span data-stu-id="aaf17-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="aaf17-145">Vyberte používateľa v zozname.</span><span class="sxs-lookup"><span data-stu-id="aaf17-145">Select a user from the list.</span></span>
1. <span data-ttu-id="aaf17-146">Pre vybratého používateľa vyberte položku **Prehľad** a potom na paneli príkazov kliknite na položku **vytvoriť nové heslo**.</span><span class="sxs-lookup"><span data-stu-id="aaf17-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="aaf17-147">Postupujte podľa pokynov na obrazovke.</span><span class="sxs-lookup"><span data-stu-id="aaf17-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="aaf17-148">Obnoví sa len prostredníctvom zápisom hesla podpory platformy Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="aaf17-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="aaf17-149">**Pri resetovaní hesla lokálneho používateľa na portáli pre správcov služieb Office 365 alebo v mobilnej aplikácii balíka Office 365 sa používateľ stále nedokáže prihlásiť**</span><span class="sxs-lookup"><span data-stu-id="aaf17-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="aaf17-150">Na tomto portáli nie je podporovaná zápisom hesla.</span><span class="sxs-lookup"><span data-stu-id="aaf17-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="aaf17-151">Opätovné vytvorenie nového hesla používateľa na portáli Azure – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="aaf17-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

