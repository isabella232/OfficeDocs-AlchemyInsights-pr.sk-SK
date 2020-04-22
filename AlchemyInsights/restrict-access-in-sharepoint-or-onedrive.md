---
title: Obmedzenie prístupu v SharePointe alebo OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715899"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="af240-102">Obmedzenie prístupu v SharePointe alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="af240-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="af240-103">V službe SharePoint a OneDrive obmedzujete prístup k položkám, ako sú súbory, priečinky a zoznamy, a to poskytnutím prístupu len skupinám alebo jednotlivcom, ktorým chcete mať prístup.</span><span class="sxs-lookup"><span data-stu-id="af240-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="af240-104">V predvolenom nastavení povolenia SharePoint sú zdedené z vyššej v hierarchii.</span><span class="sxs-lookup"><span data-stu-id="af240-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="af240-105">Takže súbor zdedí svoje povolenia z priečinka, ktorý zdedí svoje povolenia z knižnice, ktorá zdedí svoje povolenia z webu.</span><span class="sxs-lookup"><span data-stu-id="af240-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="af240-106">Môžete zdieľať na vyššej úrovni (napríklad zdieľaním celej lokality) a potom porušiť dedičnosť, ak nechcete zdieľať všetky položky na lokalite.</span><span class="sxs-lookup"><span data-stu-id="af240-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="af240-107">Avšak, neodporúčame to, pretože to robí zachovanie povolenia zložitejšie a mätúce v budúcnosti.</span><span class="sxs-lookup"><span data-stu-id="af240-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="af240-108">Tu je to, čo by ste mohli urobiť miesto:</span><span class="sxs-lookup"><span data-stu-id="af240-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="af240-109">Ak napríklad chcete zdieľať všetok obsah priečinka okrem jedného súboru, premiestnite tento súbor na nové miesto, ktoré nie je zdieľané.</span><span class="sxs-lookup"><span data-stu-id="af240-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="af240-110">Ak máte v priečinku dva podpriečinky a chcete zdieľať jeden podpriečinok so skupinami a a B a povoliť iba zoskupovanie prístupu k druhému podpriečinku, zdieľajte nadradený priečinok so skupinou a a pridajte skupinu B do prvého podpriečinka.</span><span class="sxs-lookup"><span data-stu-id="af240-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="af240-111">Zastavenie zdieľania súboru alebo priečinka</span><span class="sxs-lookup"><span data-stu-id="af240-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

