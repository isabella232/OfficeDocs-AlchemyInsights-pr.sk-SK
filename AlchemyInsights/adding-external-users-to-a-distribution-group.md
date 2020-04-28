---
title: Pridanie externých používateľov do distribučnej skupiny
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910947"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="53e3d-102">Pridanie externých používateľov do distribučnej skupiny</span><span class="sxs-lookup"><span data-stu-id="53e3d-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="53e3d-103">Pridanie externého kontaktu do distribučnej skupiny (DG) je dvojfázový proces:</span><span class="sxs-lookup"><span data-stu-id="53e3d-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="53e3d-104">Vytvorenie poštového kontaktu pre externého používateľa:</span><span class="sxs-lookup"><span data-stu-id="53e3d-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="53e3d-105">V centre spravovania prejdite na stránku **Používatelia** > [kontaktov](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="53e3d-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="53e3d-106">Vyberte položku **Pridať kontakt**.</span><span class="sxs-lookup"><span data-stu-id="53e3d-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="53e3d-107">Zadajte informácie o kontakte a vyberte položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="53e3d-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="53e3d-108">Pridajte poštový kontakt do svojho GR:</span><span class="sxs-lookup"><span data-stu-id="53e3d-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="53e3d-109">V centre spravovania prejdite na[Groups](https://admin.microsoft.com/adminportal/home#/groups)  >  **stránku skupiny skupín**.</span><span class="sxs-lookup"><span data-stu-id="53e3d-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="53e3d-110">Nájdite GR, do ktorého chcete pridať externého používateľa, a vyberte ho, ak chcete otvoriť dialógové okno úprav.</span><span class="sxs-lookup"><span data-stu-id="53e3d-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="53e3d-111">Na karte **členovia** vyberte položku **Zobraziť všetky a spravovať členov**.</span><span class="sxs-lookup"><span data-stu-id="53e3d-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="53e3d-112">Vyberte položku **pridať členov**.</span><span class="sxs-lookup"><span data-stu-id="53e3d-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="53e3d-113">Vyberte poštový kontakt, ktorý ste vytvorili v predchádzajúcom kroku, a potom vyberte položku **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="53e3d-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="53e3d-114">Ak po týchto krokoch Externí používatelia nemôžu odosielať e-maily do GR alebo neprijímajú e-maily z nej, mohlo by to byť, že GR je označené, že povolí iba e-maily od interných používateľov.</span><span class="sxs-lookup"><span data-stu-id="53e3d-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="53e3d-115">Môžete skontrolovať túto konfiguráciu a opraviť ju podľa návodu [tu](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="53e3d-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="53e3d-116">**Poznámka:** Tieto pokyny neplatia, ak typ skupiny je "Microsoft 365 skupina" namiesto "distribučnej skupiny."</span><span class="sxs-lookup"><span data-stu-id="53e3d-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="53e3d-117">V takom prípade môžete externý používateľ pridať priamo do skupiny z programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="53e3d-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="53e3d-118">Podrobné informácie o Microsoft 365 skupiny hostí, rovnako ako návod na pridávanie externých hostí možno nájsť v [tomto článku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="53e3d-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  