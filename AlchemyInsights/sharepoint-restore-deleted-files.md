---
title: Obnovenie odstráneného súboru alebo priečinka
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797563"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="f17ab-102">Obnovenie odstráneného súboru alebo priečinka</span><span class="sxs-lookup"><span data-stu-id="f17ab-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="f17ab-103">SharePoint Online uchováva zálohy všetkého obsahu počas ďalších 14 dní od samotného odstránenia.</span><span class="sxs-lookup"><span data-stu-id="f17ab-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="f17ab-104">Ak nie je možné obnoviť obsah prostredníctvom koša ani obnovenia súborov, správca sa môže obrátiť na oddelenie technickej podpory spoločnosti Microsoft a požiadať o obnovenie kedykoľvek v okne 14 dní.</span><span class="sxs-lookup"><span data-stu-id="f17ab-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="f17ab-105">Obnovenie zo záloh je možné vykonať len pre kolekcie lokalít alebo podlokality, nie pre konkrétne súbory, zoznamy alebo knižnice.</span><span class="sxs-lookup"><span data-stu-id="f17ab-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="f17ab-106">Po odstránení položky alebo lokality zo služby SharePoint sa táto položka neodstráni okamžite.</span><span class="sxs-lookup"><span data-stu-id="f17ab-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="f17ab-107">Odstránené položky sa na určitý čas premiestnia do Koša.</span><span class="sxs-lookup"><span data-stu-id="f17ab-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="f17ab-108">Počas tohto času môžete odstránené položky obnoviť do pôvodného umiestnenia.</span><span class="sxs-lookup"><span data-stu-id="f17ab-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="f17ab-109">Ďalšie informácie nájdete na prepojeniach nižšie.</span><span class="sxs-lookup"><span data-stu-id="f17ab-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="f17ab-110">[Obnovte položky v koši na lokalite SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="f17ab-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="f17ab-111">Obnovenie odstránených súborov alebo priečinkov vo OneDrive</span><span class="sxs-lookup"><span data-stu-id="f17ab-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="f17ab-112">Obnovenie odstránenej kolekcie lokalít (vrátane skupiny, komunikácie a iných lokalít)</span><span class="sxs-lookup"><span data-stu-id="f17ab-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="f17ab-113">Obnovenie odstránenej lokality OneDrive</span><span class="sxs-lookup"><span data-stu-id="f17ab-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="f17ab-114">Ak ide o hromadnú akciu Kôš, správcovia môžu zvážiť používanie [služby SharePoint Online PnP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="f17ab-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="f17ab-115">**Funkcia obnovenia súborov**</span><span class="sxs-lookup"><span data-stu-id="f17ab-115">**Files Restore feature**</span></span>

<span data-ttu-id="f17ab-116">Ak je veľa súborov vo OneDrive alebo SharePointe odstránených, prepísaných, poškodených alebo infikovaných malvérom, môžete celú knižnicu služby OneDrive alebo SharePoint obnoviť na predchádzajúcu dobu pomocou funkcie Obnovenie súborov.</span><span class="sxs-lookup"><span data-stu-id="f17ab-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="f17ab-117">Obnovenie knižnice OneDrivu</span><span class="sxs-lookup"><span data-stu-id="f17ab-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="f17ab-118">Obnovenie knižnice dokumentov</span><span class="sxs-lookup"><span data-stu-id="f17ab-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

