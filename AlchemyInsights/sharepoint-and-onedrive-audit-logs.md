---
title: Klasické zostavy denníkov auditu SharePointu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662223"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="c2518-102">Denníky auditu SharePointu a OneDrivu</span><span class="sxs-lookup"><span data-stu-id="c2518-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="c2518-103">Klasické denníky auditu SharePointu</span><span class="sxs-lookup"><span data-stu-id="c2518-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="c2518-104">Audity SPO Legacy sa sťahovali do jednotného denníka auditu (UAL).</span><span class="sxs-lookup"><span data-stu-id="c2518-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="c2518-105">Všetky staršie správy o audite SPO budú teraz poháňané prostredníctvom funkcie UAL a staršie audítorské signály sa migrujú do funkcie UAL.</span><span class="sxs-lookup"><span data-stu-id="c2518-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="c2518-106">Kľúčové zmeny:</span><span class="sxs-lookup"><span data-stu-id="c2518-106">Key changes:</span></span>

* <span data-ttu-id="c2518-107">Orezávanie nie je k dispozícii ako možnosť.</span><span class="sxs-lookup"><span data-stu-id="c2518-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="c2518-108">Výber konkrétnych udalostí na audit nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="c2518-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="c2518-109">Ak chcete zobraziť celý zoznam auditovaných udalostí, ktoré sú k dispozícii na základe predvoleného nastavenia, pozrite si [Tento dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) .</span><span class="sxs-lookup"><span data-stu-id="c2518-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="c2518-110">Možnosť **umiestnenie** v časti **prispôsobené zostavy** nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="c2518-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="c2518-111">Možnosť **Otvoriť alebo stiahnuť dokumenty** nie je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="c2518-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="c2518-112">Konfigurácia nastavenia auditu pre kolekciu lokalít</span><span class="sxs-lookup"><span data-stu-id="c2518-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="c2518-113">Moderné zjednotené denníky auditu SharePointu a OneDrivu z dodržiavania súladu</span><span class="sxs-lookup"><span data-stu-id="c2518-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="c2518-114">Zapnutie a vypnutie zjednoteného zapisovania do denníka auditu</span><span class="sxs-lookup"><span data-stu-id="c2518-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="c2518-115">V rámci SharePointu alebo OneDrivu sa nevyžaduje žiadna ďalšia konfigurácia.</span><span class="sxs-lookup"><span data-stu-id="c2518-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="c2518-116">Použite vyhľadávanie zapisovanie do denníka auditu na kontrolu aktivity súborov, priečinkov, používateľov, povolení:</span><span class="sxs-lookup"><span data-stu-id="c2518-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="c2518-117">Aktivity týkajúce sa súborov a stránok</span><span class="sxs-lookup"><span data-stu-id="c2518-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="c2518-118">Aktivity priečinka</span><span class="sxs-lookup"><span data-stu-id="c2518-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="c2518-119">Aktivity týkajúce sa zdieľania a žiadosti o prístup</span><span class="sxs-lookup"><span data-stu-id="c2518-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="c2518-120">Aktivity synchronizácie</span><span class="sxs-lookup"><span data-stu-id="c2518-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="c2518-121">Aktivity týkajúce sa správy lokality</span><span class="sxs-lookup"><span data-stu-id="c2518-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="c2518-122">Ďalšie informácie o tom, ako získať tieto udalosti, nájdete [v téme Vyhľadávanie v denníku auditu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="c2518-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
