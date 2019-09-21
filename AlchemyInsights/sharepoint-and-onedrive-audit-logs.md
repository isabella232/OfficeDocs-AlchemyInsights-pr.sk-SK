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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068038"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="11363-102">Denníky auditu služby SharePoint a OneDrive</span><span class="sxs-lookup"><span data-stu-id="11363-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="11363-103">**SharePoint a OneDrive moderné Unified audit denníky z súladu**</span><span class="sxs-lookup"><span data-stu-id="11363-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="11363-104">Zapnutie/vypnutie zapisovania do denníka zjednoteného auditu</span><span class="sxs-lookup"><span data-stu-id="11363-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="11363-105">V SharePointe alebo OneDrive sa nevyžaduje žiadna dodatočná konfigurácia.</span><span class="sxs-lookup"><span data-stu-id="11363-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="11363-106">Použite auditovanie zapisovania do denníka na kontrolu aktivity súborov, priečinkov, používateľov, povolení:</span><span class="sxs-lookup"><span data-stu-id="11363-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="11363-107">Aktivity súborov a strán</span><span class="sxs-lookup"><span data-stu-id="11363-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="11363-108">Aktivity priečinkov</span><span class="sxs-lookup"><span data-stu-id="11363-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="11363-109">Aktivity zdieľania a prístupu k žiadosti o prístup</span><span class="sxs-lookup"><span data-stu-id="11363-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="11363-110">Synchronizačné aktivity</span><span class="sxs-lookup"><span data-stu-id="11363-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="11363-111">Činnosti správy lokality</span><span class="sxs-lookup"><span data-stu-id="11363-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="11363-112">Ďalšie informácie o možnostiach získania týchto udalostí nájdete [v téme Vyhľadávanie v denníku auditu](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="11363-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="11363-113">**Denníky auditu služby SharePoint Classic**</span><span class="sxs-lookup"><span data-stu-id="11363-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="11363-114">Migrovali sme auditovanie SPO Legacy do zjednoteného denníka auditu (UAL).</span><span class="sxs-lookup"><span data-stu-id="11363-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="11363-115">To v podstate znamená, že všetky SPO staršie audítorské správy budú teraz napájané prostredníctvom UAL a staršie audítorské signály boli presunuté do UAL.</span><span class="sxs-lookup"><span data-stu-id="11363-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="11363-116">Kľúčové zmeny:</span><span class="sxs-lookup"><span data-stu-id="11363-116">Key changes:</span></span>

- <span data-ttu-id="11363-117">Orezávanie ako schopnosť nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="11363-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="11363-118">Sekcia, kde si vyberiete konkrétne udalosti na auditovanie, nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="11363-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="11363-119">Úplný zoznam auditovaných udalostí, ktoré sú v predvolenom nastavení k dispozícii, nájdete [v tomto dokumente](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) .</span><span class="sxs-lookup"><span data-stu-id="11363-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="11363-120">Možnosť "umiestnenie" v časti **prispôsobené prehľady** nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="11363-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="11363-121">Udalosti "otváranie alebo preberanie dokumentov" nie sú k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="11363-121">“Opening or downloading documents” events is NOT available.</span></span> 

