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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708077"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="ca077-102">Chyby synchronizácie spôsobené duplicitnými objektmi</span><span class="sxs-lookup"><span data-stu-id="ca077-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="ca077-103">Pri dokončení synchronizácie adresárov v programe Microsoft 365 sa môže zobraziť jedno z nasledujúcich chybových hlásení:</span><span class="sxs-lookup"><span data-stu-id="ca077-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="ca077-104">Nie je možné aktualizovať tento objekt v službách Microsoft Online Services, pretože nasledovné atribúty priradené k tomuto objektu majú hodnoty, ktoré už môžu byť priradené k inému objektu v lokálnom adresári.</span><span class="sxs-lookup"><span data-stu-id="ca077-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="ca077-105">Synchronizovaný objekt s rovnakou adresou proxy už existuje v adresári služieb Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="ca077-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="ca077-106">Nie je možné aktualizovať tento objekt, pretože nasledovné atribúty priradené k tomuto objektu majú hodnoty, ktoré už môžu byť priradené k inému objektu v miestnych adresárových službách: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="ca077-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="ca077-107">Ak chcete problém identifikovať a vyriešiť, Stiahnite a spustite [nástroj na sanáciu chýb nástroja IdFix DirSync](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="ca077-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="ca077-108">Ďalšie informácie nájdete v téme [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="ca077-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
