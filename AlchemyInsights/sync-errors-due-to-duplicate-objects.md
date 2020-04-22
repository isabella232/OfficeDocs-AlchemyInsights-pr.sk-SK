---
title: 902 (chyby synchronizácie z dôvodu duplicitných objektov)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767150"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="4c50b-102">Chyby synchronizácie spôsobené duplicitnými objektmi</span><span class="sxs-lookup"><span data-stu-id="4c50b-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="4c50b-103">Pri dokončení synchronizácie adresárov v Microsoft 365 sa môže zobraziť jedno z nasledujúcich chybových hlásení:</span><span class="sxs-lookup"><span data-stu-id="4c50b-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="4c50b-104">Nie je možné aktualizovať tento objekt v službách online spoločnosti Microsoft, pretože nasledujúce atribúty priradené k tomuto objektu majú hodnoty, ktoré už môžu byť priradené k inému objektu v lokálnom adresári.</span><span class="sxs-lookup"><span data-stu-id="4c50b-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="4c50b-105">Synchronizovaný objekt s rovnakou adresou servera proxy už existuje v adresári služieb Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="4c50b-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="4c50b-106">Tento objekt sa nedá aktualizovať, pretože nasledujúce atribúty priradené k tomuto objektu majú hodnoty, ktoré už môžu byť priradené k inému objektu v miestnych adresárových službách: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4c50b-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="4c50b-107">Identifikovať a opraviť problém, prevezmite a spustite [Nástroj IdFix DirSync chyba Remediation](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="4c50b-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="4c50b-108">Ďalšie informácie nájdete na [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="4c50b-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
