---
title: Obmedzenie prístupu v SharePointe alebo OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551466"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="bee96-102">Obmedzenie prístupu v SharePointe alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="bee96-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="bee96-103">V službe SharePoint a OneDrive obmedzujete prístup k položkám, ako sú súbory, priečinky a zoznamy, a to poskytnutím prístupu len skupinám alebo jednotlivcom, ktorým chcete mať prístup.</span><span class="sxs-lookup"><span data-stu-id="bee96-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="bee96-104">V predvolenom nastavení povolenia SharePoint sú zdedené z vyššej v hierarchii.</span><span class="sxs-lookup"><span data-stu-id="bee96-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="bee96-105">Takže súbor zdedí svoje povolenia z priečinka, ktorý zdedí svoje povolenia z knižnice, ktorá zdedí svoje povolenia z webu.</span><span class="sxs-lookup"><span data-stu-id="bee96-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="bee96-106">Môžete zdieľať na vyššej úrovni (napríklad zdieľaním celej lokality) a potom porušiť dedičnosť, ak nechcete zdieľať všetky položky na lokalite.</span><span class="sxs-lookup"><span data-stu-id="bee96-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="bee96-107">Avšak, neodporúčame to, pretože to robí zachovanie povolenia zložitejšie a mätúce v budúcnosti.</span><span class="sxs-lookup"><span data-stu-id="bee96-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="bee96-108">Tu je to, čo by ste mohli urobiť miesto:</span><span class="sxs-lookup"><span data-stu-id="bee96-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="bee96-109">Ak napríklad chcete zdieľať všetok obsah priečinka okrem jedného súboru, premiestnite tento súbor na nové miesto, ktoré nie je zdieľané.</span><span class="sxs-lookup"><span data-stu-id="bee96-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="bee96-110">Ak máte v priečinku dva podpriečinky a chcete zdieľať jeden podpriečinok so skupinami a a B a povoliť iba zoskupovanie prístupu k druhému podpriečinku, zdieľajte nadradený priečinok so skupinou a a pridajte skupinu B do prvého podpriečinka.</span><span class="sxs-lookup"><span data-stu-id="bee96-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="bee96-111">Zastavenie zdieľania súboru alebo priečinka</span><span class="sxs-lookup"><span data-stu-id="bee96-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

