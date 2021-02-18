---
title: Správa externých nastavení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294435"
---
# <a name="managing-external-settings"></a><span data-ttu-id="bb31c-102">Správa externých nastavení</span><span class="sxs-lookup"><span data-stu-id="bb31c-102">Managing External Settings</span></span>

<span data-ttu-id="bb31c-103">**Oznámenie**</span><span class="sxs-lookup"><span data-stu-id="bb31c-103">**Announcement**</span></span>

- <span data-ttu-id="bb31c-104">[Odmietanie podpory pri prihlasovaní na webové stránky od spoločnosti Google od 4. januára 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="bb31c-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="bb31c-105">Otestujte, či sú vaše aplikácie ovplyvnené podľa pokynov spoločnosti Google v oblasti testovania kompatibility</span><span class="sxs-lookup"><span data-stu-id="bb31c-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="bb31c-106">Uistite sa, že pri prihlasovaní používateľov pomocou používateľských kont Google používate systémové webové zobrazenie alebo systémový prehliadač</span><span class="sxs-lookup"><span data-stu-id="bb31c-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="bb31c-107">**Spravovanie nastavení pozvánok**</span><span class="sxs-lookup"><span data-stu-id="bb31c-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="bb31c-108">Potvrďte, že ste [nakonfigurovali nastavenie externej spolupráce](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) , aby sa umožnilo príslušným ľuďom odosielať pozvánky.</span><span class="sxs-lookup"><span data-stu-id="bb31c-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="bb31c-109">**Správa povolení na prístup používateľov hosťa**</span><span class="sxs-lookup"><span data-stu-id="bb31c-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="bb31c-110">Globálny správcovia môžu spravovať povolenia hosťovského prístupu v adresári prostredníctvom portálu Azure konfiguráciou povolení na prístup hostí na stránke externého nastavenia spolupráce.</span><span class="sxs-lookup"><span data-stu-id="bb31c-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="bb31c-111">Ďalšie [informácie o tomto nastavení](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="bb31c-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="bb31c-112">Ak chcete, aby mali hostia prístup k aplikáciám, ako sú napríklad aplikácie teams alebo SharePoint, potvrďte, že ste nakonfigurovali tieto aplikácie, aby umožnili prístup hostí.</span><span class="sxs-lookup"><span data-stu-id="bb31c-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="bb31c-113">Ďalšie informácie o [nastaveniach tímov](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) a [SharePointe](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="bb31c-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="bb31c-114">**Konfigurovanie pozvánok:**</span><span class="sxs-lookup"><span data-stu-id="bb31c-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="bb31c-115">Povolenie externej spolupráce B2B a spravovanie osôb, ktoré môžu pozvať hostí</span><span class="sxs-lookup"><span data-stu-id="bb31c-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="bb31c-116">Povolenie alebo blokovanie pozvánok používateľom z konkrétnych organizácií</span><span class="sxs-lookup"><span data-stu-id="bb31c-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="bb31c-117">**Konfigurovanie povolených poskytovateľov identity:**</span><span class="sxs-lookup"><span data-stu-id="bb31c-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="bb31c-118">Federácia služby Google</span><span class="sxs-lookup"><span data-stu-id="bb31c-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="bb31c-119">Priama federácia</span><span class="sxs-lookup"><span data-stu-id="bb31c-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="bb31c-120">Overenie e-mailu jedným časovým heslom</span><span class="sxs-lookup"><span data-stu-id="bb31c-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
