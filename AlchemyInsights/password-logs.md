---
title: Denníky hesiel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527181"
---
# <a name="password-logs"></a><span data-ttu-id="c0cca-102">Denníky hesiel</span><span class="sxs-lookup"><span data-stu-id="c0cca-102">Password logs</span></span>

<span data-ttu-id="c0cca-103">**Mám problémy s prístupom k denníkom auditu na vytvorenie nového hesla**</span><span class="sxs-lookup"><span data-stu-id="c0cca-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="c0cca-104">Ak chcete riešiť problémy týkajúce sa prístupu k denníkom auditu na vytvorenie nového hesla, vykonajte nasledujúci krok:</span><span class="sxs-lookup"><span data-stu-id="c0cca-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="c0cca-105">Uistite sa, že máte povolenie na zobrazenie denníkov auditu.</span><span class="sxs-lookup"><span data-stu-id="c0cca-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="c0cca-106">Povolené sú len tieto roly:</span><span class="sxs-lookup"><span data-stu-id="c0cca-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="c0cca-107">Globálny správca</span><span class="sxs-lookup"><span data-stu-id="c0cca-107">Global administrator</span></span>
 - <span data-ttu-id="c0cca-108">Správca zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="c0cca-108">Security administrator</span></span>
 - <span data-ttu-id="c0cca-109">Čítačka zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="c0cca-109">Security reader</span></span>

<span data-ttu-id="c0cca-110">**Chcem Zobraziť všetky udalosti auditu obnovenia nového hesla od začiatku nasadeného času**</span><span class="sxs-lookup"><span data-stu-id="c0cca-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="c0cca-111">V zostavách za posledných 30 dní sú uložené až 120 000 heslá na vytvorenie nového hesla alebo udalosti registrácie.</span><span class="sxs-lookup"><span data-stu-id="c0cca-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="c0cca-112">Tento maximálny limit sa vzťahuje na používateľské rozhranie pri sťahovaní súboru CSV.</span><span class="sxs-lookup"><span data-stu-id="c0cca-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="c0cca-113">udalosti 1 000 000 sú k dispozícii v prostredí PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c0cca-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="c0cca-114">Ďalšie informácie nájdete v prepojeniach nižšie:</span><span class="sxs-lookup"><span data-stu-id="c0cca-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="c0cca-115">Samoobslužné udalosti na vytvorenie nového hesla zo zostáv služby Azure AD a rozhrania API udalostí</span><span class="sxs-lookup"><span data-stu-id="c0cca-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c0cca-116">Ako stiahnuť nové heslo registrácia udalosti rýchlo s prostredím PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0cca-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="c0cca-117">**Chcem sa dozvedieť viac o možnostiach vytvárania správ na vytvorenie nového hesla**</span><span class="sxs-lookup"><span data-stu-id="c0cca-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="c0cca-118">Skontrolujte, kto registruje alebo nastavuje heslá pomocou denníkov auditu obnovenia nového hesla Azure AD na portáli Azure v časti **Používatelia a skupiny**.</span><span class="sxs-lookup"><span data-stu-id="c0cca-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="c0cca-119">Ďalšie informácie nájdete v týchto prepojeniach:</span><span class="sxs-lookup"><span data-stu-id="c0cca-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="c0cca-120">Prehľad zostáv na vytvorenie nového hesla</span><span class="sxs-lookup"><span data-stu-id="c0cca-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c0cca-121">Zobrazenie zostáv na vytvorenie nového hesla na portáli Azure</span><span class="sxs-lookup"><span data-stu-id="c0cca-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c0cca-122">Samoobslužné udalosti na vytvorenie nového hesla zo zostáv služby Azure AD a rozhrania API udalostí</span><span class="sxs-lookup"><span data-stu-id="c0cca-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="c0cca-123">Ako stiahnuť nové heslo registrácia udalosti rýchlo s prostredím PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0cca-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


