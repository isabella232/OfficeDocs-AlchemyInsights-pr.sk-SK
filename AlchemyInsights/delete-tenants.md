---
title: Odstrániť nájomníka
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564881"
---
# <a name="delete-tenant"></a><span data-ttu-id="2973e-102">Odstrániť nájomníka</span><span class="sxs-lookup"><span data-stu-id="2973e-102">Delete tenant</span></span>

<span data-ttu-id="2973e-103">Ak chcete odstrániť Azure AD, zabezpečte:</span><span class="sxs-lookup"><span data-stu-id="2973e-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="2973e-104">Ste globálnym správcom v adresári.</span><span class="sxs-lookup"><span data-stu-id="2973e-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="2973e-105">NIE ste prihlásení s kontom, ktoré má predvolený adresár, napríklad contoso.onmicrosoft.com, v prihlasovacom konte, ako je napríklad admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="2973e-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="2973e-106">Pred odstránením odstráňte všetky aktívne aplikácie v adresári.</span><span class="sxs-lookup"><span data-stu-id="2973e-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="2973e-107">Ak chcete odstrániť aktívne aplikácie, prejdite na položku registrácie aplikácií a odstráňte existujúce aplikácie.</span><span class="sxs-lookup"><span data-stu-id="2973e-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="2973e-108">Neexistujú žiadne aktívne predplatné na žiadne služby Microsoft Online Services, ako je napríklad Microsoft Azure, Office 365 alebo Azure AD Premium, ktoré sú priradené k adresáru.</span><span class="sxs-lookup"><span data-stu-id="2973e-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="2973e-109">Prenášajte predplatné alebo Zrýchlite zrušenie aktívnych predplatných prostredníctvom podpory Azure a fakturácie.</span><span class="sxs-lookup"><span data-stu-id="2973e-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="2973e-110">Ďalšie informácie o zrušení predplatného na Office 365 a Azure.</span><span class="sxs-lookup"><span data-stu-id="2973e-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="2973e-111">Pokyny na priradenie alebo Pridanie existujúceho predplatného nájomníkovi nájdete v téme [Priradenie alebo pridanie predplatného Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="2973e-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="2973e-112">K dispozícii nie sú žiadne aktívne licencie.</span><span class="sxs-lookup"><span data-stu-id="2973e-112">There are no Active license.</span></span> <span data-ttu-id="2973e-113">Ak chcete odstrániť licencie, pozrite si tému [Odstránenie predplatného na odstránenie licencie](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="2973e-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="2973e-114">Pri pokuse o odstránenie Azure AD sa nenachádzajú žiadne ďalšie aktívni používatelia v adresári okrem seba ako globálny správca.</span><span class="sxs-lookup"><span data-stu-id="2973e-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="2973e-115">Odstráňte všetkých ostatných aktívnych používateľov a všetky závislosti na vlastnom názve domény v nájomníkovi budú tiež potrebné odstrániť, ako napríklad používatelia vytvorené pomocou admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="2973e-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="2973e-116">Ďalšie podrobnosti nájdete v téme postup:</span><span class="sxs-lookup"><span data-stu-id="2973e-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="2973e-117">Odstránenie služby Azure Active Directory alebo predplatného nájdete v téme [Odstránenie Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="2973e-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="2973e-118">Odstraňujú sa aplikácie v adresári, pozrite si tému [odstránenie aplikácií](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="2973e-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
