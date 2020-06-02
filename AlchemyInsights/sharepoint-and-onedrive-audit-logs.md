---
title: Klasické zostavy denníka auditu SharePointu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509615"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="7f975-102">Denníky auditu SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="7f975-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="7f975-103">Klasické denníky auditu lokality SharePoint</span><span class="sxs-lookup"><span data-stu-id="7f975-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="7f975-104">SPO staršie auditovanie migrovala do unified audit auditu (UAL).</span><span class="sxs-lookup"><span data-stu-id="7f975-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="7f975-105">Všetky správy o audite spo staršie správy budú teraz napájané prostredníctvom UAL a staršie signály auditu boli premiestnené do UAL.</span><span class="sxs-lookup"><span data-stu-id="7f975-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="7f975-106">Kľúčové zmeny:</span><span class="sxs-lookup"><span data-stu-id="7f975-106">Key changes:</span></span>

* <span data-ttu-id="7f975-107">Orezávanie nie je k dispozícii ako schopnosť.</span><span class="sxs-lookup"><span data-stu-id="7f975-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="7f975-108">Výber konkrétnych udalostí na audit nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="7f975-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="7f975-109">Úplný zoznam kontrolovaných udalostí, ktoré sú predvolene k dispozícii, nájdete v [tomto dokumente.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="7f975-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="7f975-110">Možnosť **Umiestnenie** v časti **Prispôsobené zostavy** nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="7f975-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="7f975-111">Možnosť **Otváranie alebo preberanie udalostí dokumentov** nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="7f975-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="7f975-112">Konfigurácia nastavenia auditu pre kolekciu lokalít</span><span class="sxs-lookup"><span data-stu-id="7f975-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="7f975-113">Denníky moderného zjednoteného auditu SharePointu a OneDrivu zo súladu</span><span class="sxs-lookup"><span data-stu-id="7f975-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="7f975-114">Zapnutie/vypnutie zapisovania do denníka zjednoteného auditu</span><span class="sxs-lookup"><span data-stu-id="7f975-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="7f975-115">V SharePointe alebo OneDrive sa nevyžaduje žiadna ďalšia konfigurácia.</span><span class="sxs-lookup"><span data-stu-id="7f975-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="7f975-116">Pomocou vyhľadávania zapisovania do denníka auditu skontrolujte aktivitu súborov, priečinkov, používateľov, povolení:</span><span class="sxs-lookup"><span data-stu-id="7f975-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="7f975-117">Aktivity súborov a stránok</span><span class="sxs-lookup"><span data-stu-id="7f975-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="7f975-118">Aktivity priečinkov</span><span class="sxs-lookup"><span data-stu-id="7f975-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="7f975-119">Zdieľanie a prístup k činnostiam so žiadosťou</span><span class="sxs-lookup"><span data-stu-id="7f975-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="7f975-120">Činnosti synchronizácie</span><span class="sxs-lookup"><span data-stu-id="7f975-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="7f975-121">Činnosti správy staveniska</span><span class="sxs-lookup"><span data-stu-id="7f975-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="7f975-122">Ďalšie informácie o načítanie týchto udalostí nájdete v téme [Vyhľadávanie v denníku auditu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="7f975-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
