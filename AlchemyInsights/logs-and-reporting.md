---
title: Denníky a nahlasovanie
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036012"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="c0ac5-102">Denníky a nahlasovanie</span><span class="sxs-lookup"><span data-stu-id="c0ac5-102">Logs and Reporting</span></span>

<span data-ttu-id="c0ac5-103">Najčastejšie otázky týkajúce sa zostavy [služby Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) nájdete v téme Najčastejšie otázky týkajúce sa vytvárania zostavy služby Azure AD (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c0ac5-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="c0ac5-104">Ďalšie informácie nájdete v téme [zostavy služby Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span><span class="sxs-lookup"><span data-stu-id="c0ac5-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="c0ac5-105">**Riešenie problémov s auditom**</span><span class="sxs-lookup"><span data-stu-id="c0ac5-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="c0ac5-106">Ak sa vyskytnú problémy s niektorými aktivitami auditu a chýbajúca aktivita je v tomto [zozname](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), požiadajte o pomoc lístok technickej podpory.</span><span class="sxs-lookup"><span data-stu-id="c0ac5-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="c0ac5-107">Ak máte problémy so zobrazením všetkých denníkov auditu v nájomníkovi, požiadajte o pomoc lístok technickej podpory.</span><span class="sxs-lookup"><span data-stu-id="c0ac5-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="c0ac5-108">Ak sa vaše audity nezobrazujú okamžite na portáli Azure, pozrite si [informácie o latencii](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) a pohľadajte lístok podpory, ak oneskorenie presiahne zdokumentovaný čas oneskorenia.</span><span class="sxs-lookup"><span data-stu-id="c0ac5-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="c0ac5-109">Uchovanie denníkov aktivít služby Azure AD</span><span class="sxs-lookup"><span data-stu-id="c0ac5-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="c0ac5-110">Ak sa nezobrazuje celý audit pre vybratý rozsah dátumov, môžete si stiahnuť až 250K riadky (zoradené podľa najnovších) prihlasovacích modulov z portálu Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="c0ac5-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="c0ac5-111">Ďalšie informácie nájdete v téme [stiahnutie aktivít auditovania](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="c0ac5-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="c0ac5-112">**Riešenie problémov s prihlásením**</span><span class="sxs-lookup"><span data-stu-id="c0ac5-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="c0ac5-113">Ak máte licenciu na verziu Azure AD Premium (P1 alebo P2) pre vášho nájomníka, môžete zobraziť len posledných 30 dní údajov.</span><span class="sxs-lookup"><span data-stu-id="c0ac5-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="c0ac5-114">Prihlasovacie moduly sú k dispozícii len pre nájomníkov služby Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="c0ac5-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="c0ac5-115">Nie je k dispozícii pre voľných alebo základných licencovaných nájomníkov.</span><span class="sxs-lookup"><span data-stu-id="c0ac5-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="c0ac5-116">Ak má váš nájomník licenciu Premium P1 a nevidíte prihlasovacie údaje, pozrite si [informácie o latencii](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) a zapíšte si lístok podpory, ak oneskorenie presiahne zdokumentovaný čas oneskorenia.</span><span class="sxs-lookup"><span data-stu-id="c0ac5-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="c0ac5-117">Ak sa nezobrazujú všetky prihlásenia pre rozsah dátumov, ktoré ste vybrali, Všimnite si, že si môžete stiahnuť až 250K riadky (zoradené podľa najnovších) prihlasovacích modulov zo služby Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="c0ac5-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="c0ac5-118">Ďalšie informácie nájdete v téme [stiahnutie aktivít s prihlásením](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="c0ac5-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="c0ac5-119">**Riešenie problémov so správami zabezpečenia (používatelia s príznakom riziko, riskantné prihlásenie)**</span><span class="sxs-lookup"><span data-stu-id="c0ac5-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="c0ac5-120">Používatelia s príznakom pre zostavu zabezpečenia rizika</span><span class="sxs-lookup"><span data-stu-id="c0ac5-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="c0ac5-121">Hlásenie riskantné prihlásenia na portáli Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c0ac5-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="c0ac5-122">Udalosti v službe Azure Active Directory Risk</span><span class="sxs-lookup"><span data-stu-id="c0ac5-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
