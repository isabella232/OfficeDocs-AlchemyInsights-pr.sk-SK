---
title: 902 (chyby synchronizácie spôsobené duplicitnými objektmi)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737356"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="25c75-102">Chyby synchronizácie spôsobené duplicitnými objektmi</span><span class="sxs-lookup"><span data-stu-id="25c75-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="25c75-103">Pri dokončení synchronizácie adresárov v programe Microsoft 365 sa môže zobraziť jedno z nasledujúcich chybových hlásení:</span><span class="sxs-lookup"><span data-stu-id="25c75-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="25c75-104">Nie je možné aktualizovať tento objekt v službách Microsoft Online Services, pretože nasledovné atribúty priradené k tomuto objektu majú hodnoty, ktoré už môžu byť priradené k inému objektu v lokálnom adresári.</span><span class="sxs-lookup"><span data-stu-id="25c75-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="25c75-105">Synchronizovaný objekt s rovnakou adresou proxy už existuje v adresári služieb Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="25c75-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="25c75-106">Nie je možné aktualizovať tento objekt, pretože nasledovné atribúty priradené k tomuto objektu majú hodnoty, ktoré už môžu byť priradené k inému objektu v miestnych adresárových službách: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="25c75-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="25c75-107">Ak chcete problém identifikovať a vyriešiť, Stiahnite a spustite [nástroj na sanáciu chýb nástroja IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="25c75-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="25c75-108">Ďalšie informácie nájdete v téme [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="25c75-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
