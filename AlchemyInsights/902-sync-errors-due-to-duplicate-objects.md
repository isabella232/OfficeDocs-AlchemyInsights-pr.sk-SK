---
title: 902 (sync chyby spôsobené duplicitné objekty)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311540"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="a646f-102">Chyby synchronizácie kvôli duplicitné objekty</span><span class="sxs-lookup"><span data-stu-id="a646f-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="a646f-103">Po dokončení synchronizácie adresárov sa môže zobraziť jedno z nasledujúcich chybových hlásení:</span><span class="sxs-lookup"><span data-stu-id="a646f-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="a646f-104">Nie je možné aktualizovať tento objekt Microsoft Online Services, pretože tieto atribúty priradený objekt hodnôt už priradený iný objekt v adresári lokálnej.</span><span class="sxs-lookup"><span data-stu-id="a646f-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="a646f-105">Objekt synchronizované s rovnakou adresou servera proxy už existuje v adresári služby Online spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a646f-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="a646f-106">Nie je možné aktualizovať objekt, pretože tieto atribúty priradený objekt hodnôt už priradený iný objekt v lokálnej adresár služieb: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a646f-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="a646f-107">Identifikovať a opraviť problém, prevezmite a spustenie nástroja [IdFix DirSync chyba sanácie nástroj](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="a646f-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="a646f-108">Ďalšie informácie nájdete v téme [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="a646f-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

