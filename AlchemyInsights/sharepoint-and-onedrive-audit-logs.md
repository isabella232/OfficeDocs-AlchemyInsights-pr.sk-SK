---
title: Klasické zostavy denníka auditu služby SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992633"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="4b4ea-102">Denníky auditu služby SharePoint a OneDrive</span><span class="sxs-lookup"><span data-stu-id="4b4ea-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="4b4ea-103">Denníky auditu služby SharePoint Classic</span><span class="sxs-lookup"><span data-stu-id="4b4ea-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="4b4ea-104">Auditovanie SPO Legacy bolo presunuté do zjednoteného denníka auditu (UAL).</span><span class="sxs-lookup"><span data-stu-id="4b4ea-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="4b4ea-105">Všetky SPO staršie audítorské správy budú teraz napájané prostredníctvom UAL a staršie audítorské signály boli migrované na UAL.</span><span class="sxs-lookup"><span data-stu-id="4b4ea-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="4b4ea-106">Kľúčové zmeny:</span><span class="sxs-lookup"><span data-stu-id="4b4ea-106">Key changes:</span></span>

* <span data-ttu-id="4b4ea-107">Orezávanie nie je k dispozícii ako schopnosť.</span><span class="sxs-lookup"><span data-stu-id="4b4ea-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="4b4ea-108">Výber konkrétnych udalostí na audit nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="4b4ea-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="4b4ea-109">Úplný zoznam auditovaných udalostí, ktoré sú predvolene k dispozícii, nájdete [v tomto dokumente](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) .</span><span class="sxs-lookup"><span data-stu-id="4b4ea-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="4b4ea-110">Možnosť **umiestnenie** v časti **prispôsobené prehľady** nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="4b4ea-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="4b4ea-111">Možnosť **otváranie alebo preberanie dokumentov** nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="4b4ea-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="4b4ea-112">Konfigurácia nastavení auditovania pre kolekciu lokalít</span><span class="sxs-lookup"><span data-stu-id="4b4ea-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="4b4ea-113">SharePoint a OneDrive moderné Unified audit denníky z súladu</span><span class="sxs-lookup"><span data-stu-id="4b4ea-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="4b4ea-114">Zapnutie/vypnutie zapisovania do denníka zjednoteného auditu</span><span class="sxs-lookup"><span data-stu-id="4b4ea-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="4b4ea-115">V SharePointe alebo OneDrive sa nevyžaduje žiadna dodatočná konfigurácia.</span><span class="sxs-lookup"><span data-stu-id="4b4ea-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="4b4ea-116">Použite auditovanie zapisovania do denníka na kontrolu aktivity súborov, priečinkov, používateľov, povolení:</span><span class="sxs-lookup"><span data-stu-id="4b4ea-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="4b4ea-117">Aktivity súborov a strán</span><span class="sxs-lookup"><span data-stu-id="4b4ea-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="4b4ea-118">Aktivity priečinkov</span><span class="sxs-lookup"><span data-stu-id="4b4ea-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="4b4ea-119">Aktivity zdieľania a prístupu k žiadosti o prístup</span><span class="sxs-lookup"><span data-stu-id="4b4ea-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="4b4ea-120">Synchronizačné aktivity</span><span class="sxs-lookup"><span data-stu-id="4b4ea-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="4b4ea-121">Činnosti správy lokality</span><span class="sxs-lookup"><span data-stu-id="4b4ea-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="4b4ea-122">Ďalšie informácie o možnostiach získania týchto udalostí nájdete [v téme Vyhľadávanie v denníku auditu](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="4b4ea-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
