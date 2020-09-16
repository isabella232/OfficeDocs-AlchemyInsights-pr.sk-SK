---
title: Obmedzenie prístupu v SharePointe alebo OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720697"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="74ad4-102">Obmedzenie prístupu v SharePointe alebo OneDrive</span><span class="sxs-lookup"><span data-stu-id="74ad4-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="74ad4-103">V SharePointe a OneDrive môžete obmedziť prístup k položkám, ako sú súbory, priečinky a zoznamy, udelením prístupu len skupinám alebo jednotlivcom, ktorým chcete mať prístup.</span><span class="sxs-lookup"><span data-stu-id="74ad4-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="74ad4-104">Povolenia v SharePointe sú predvolene zdedené z vyššie uvedených hodnôt v hierarchii.</span><span class="sxs-lookup"><span data-stu-id="74ad4-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="74ad4-105">Preto súbor dedí povolenia z priečinka, ktorý dedí povolenia z knižnice, ktorá dedí povolenia z lokality.</span><span class="sxs-lookup"><span data-stu-id="74ad4-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="74ad4-106">Ak nechcete zdieľať všetky položky na lokalite, môžete zdieľať na vyššej úrovni (napríklad zdieľaním celej lokality) a následným prerušením dedenia.</span><span class="sxs-lookup"><span data-stu-id="74ad4-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="74ad4-107">Táto skutočnosť sa však neodporúča, pretože zabezpečuje, aby sa v budúcnosti zachovali povolenia zložitejšie a mätúce.</span><span class="sxs-lookup"><span data-stu-id="74ad4-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="74ad4-108">Tu je to, čo by ste mohli urobiť namiesto toho:</span><span class="sxs-lookup"><span data-stu-id="74ad4-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="74ad4-109">Ak chcete napríklad zdieľať celý obsah priečinka s výnimkou jedného súboru, presuňte ho na nové miesto, ktoré nie je zdieľané.</span><span class="sxs-lookup"><span data-stu-id="74ad4-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="74ad4-110">Ak máte v priečinku dva podpriečinky a chcete zdieľať jeden podpriečinok so skupinami a a B a povoliť len skupinový prístup k druhému podpriečinku, zdieľajte nadradený priečinok so skupinou A a pridajte skupinu B do prvého podpriečinka.</span><span class="sxs-lookup"><span data-stu-id="74ad4-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="74ad4-111">Ukončenie zdieľania súboru alebo priečinka </span><span class="sxs-lookup"><span data-stu-id="74ad4-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

