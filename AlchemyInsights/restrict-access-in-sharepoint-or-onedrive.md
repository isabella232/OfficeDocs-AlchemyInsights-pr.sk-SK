---
title: Obmedzenie prístupu v SharePoint alebo OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311392"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="82e49-102">Obmedzenie prístupu v SharePoint alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="82e49-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="82e49-p101">V službe SharePoint a OneDrive, obmedzíte prístup do položiek, ako sú súbory, priečinky a zoznamy poskytnutím prístupu len pre skupiny alebo jednotlivcov, ktoré chcete mať prístup. Predvolene sú zdedené povolenia v SharePoint z výš v hierarchii. Takže súbor dedí jeho povolenia z priečinka, ktoré dedia jej povolenia z knižnice, ktoré dedia jej povolenia na lokalite.</span><span class="sxs-lookup"><span data-stu-id="82e49-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="82e49-p102">Môžete zdieľať na vyššej úrovni (ako napríklad zdieľaním celého webu) a potom porušiť dedenie, ak nechcete zdieľať všetky položky na stránke. Avšak, neodporúčame to, pretože to robí, udržiavanie povolenia zložitých a mätúce v budúcnosti. Tu je, čo by ste mohli urobiť namiesto toho:</span><span class="sxs-lookup"><span data-stu-id="82e49-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="82e49-109">Ak napríklad chcete zdieľať celý obsah priečinka s výnimkou jedného súboru, presunúť súbor do nového umiestnenia, ktorý nie je zdieľaný.</span><span class="sxs-lookup"><span data-stu-id="82e49-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="82e49-110">Ak máte dve podzložky v zložke, a chcete zdieľať jednu podpriečinok s skupín A a B a len skupina A prístup k druhej podpriečinok, zdieľanie nadradeného priečinka so skupinou A a pridať skupinu B prvý podpriečinok.</span><span class="sxs-lookup"><span data-stu-id="82e49-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="82e49-111">Ukončenie zdieľania súboru alebo priečinka</span><span class="sxs-lookup"><span data-stu-id="82e49-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

